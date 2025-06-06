ARG BASE_IMAGE
FROM ${BASE_IMAGE} AS builder
WORKDIR /app

# Install dumb-init - minimal process init system
RUN apt-get update && apt-get install -y --no-install-recommends dumb-init

# Copy everything from the base
# only install and build the main package and its dependencies
COPY pnpm-lock.yaml .
COPY pnpm-workspace.yaml .
COPY package.json .
COPY tsconfig.json .
COPY integrations/nestjs ./integrations/nestjs

# Mount the cache where pnpm expects it and build the main package
RUN --mount=type=cache,id=pnpm,target=~/.pnpm-store \
    pnpm --filter @scalar-examples/nestjs-api-reference-fastify install --frozen-lockfile && \
    pnpm --filter @scalar-examples/nestjs-api-reference-fastify build

FROM node:20-slim AS runner

# Copy from the previous stage to keep this image minimal
COPY --from=builder /usr/bin/dumb-init /usr/bin/dumb-init

ENV NODE_ENV production

# Use default non-root user from the node image
USER node
WORKDIR /app
RUN chown node:node /app

# Copy root node modules and any utilized packages
COPY --from=builder /app/node_modules /app/node_modules
COPY --from=builder /app/integrations/nestjs /app/integrations/nestjs

WORKDIR /app/integrations/nestjs/playground/nestjs-api-reference-fastify
# dumb-init runs as PID 1 and ensures all signals are forwarded
# to the spawned node process (ensures the server receives terminate signal)
CMD ["dumb-init", "node", "dist/main.js"]
