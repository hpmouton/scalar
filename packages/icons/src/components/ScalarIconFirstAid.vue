/* GENERATED FILE */
<script lang="ts">
export default {
  name: 'ScalarIconFirstAid',
}
</script>
<script lang="ts" setup>
import { useScalarIcon } from '@/hooks'
import type { ScalarIconProps } from '@/types'

const props = defineProps<ScalarIconProps>()

const { bind, weight } = useScalarIcon(props)
</script>
<template>
  <svg
    xmlns="http://www.w3.org/2000/svg"
    viewBox="0 0 256 256"
    fill="currentColor"
    v-bind="bind">
    <slot />
    <g v-if="weight === 'bold'">
      <path
        d="M216,84H172V40a20,20,0,0,0-20-20H104A20,20,0,0,0,84,40V84H40a20,20,0,0,0-20,20v48a20,20,0,0,0,20,20H84v44a20,20,0,0,0,20,20h48a20,20,0,0,0,20-20V172h44a20,20,0,0,0,20-20V104A20,20,0,0,0,216,84Zm-4,64H160a12,12,0,0,0-12,12v52H108V160a12,12,0,0,0-12-12H44V108H96a12,12,0,0,0,12-12V44h40V96a12,12,0,0,0,12,12h52Z" />
    </g>
    <g v-else-if="weight === 'duotone'">
      <path
        d="M224,104v48a8,8,0,0,1-8,8H160v56a8,8,0,0,1-8,8H104a8,8,0,0,1-8-8V160H40a8,8,0,0,1-8-8V104a8,8,0,0,1,8-8H96V40a8,8,0,0,1,8-8h48a8,8,0,0,1,8,8V96h56A8,8,0,0,1,224,104Z"
        opacity="0.2" />
      <path
        d="M216,88H168V40a16,16,0,0,0-16-16H104A16,16,0,0,0,88,40V88H40a16,16,0,0,0-16,16v48a16,16,0,0,0,16,16H88v48a16,16,0,0,0,16,16h48a16,16,0,0,0,16-16V168h48a16,16,0,0,0,16-16V104A16,16,0,0,0,216,88Zm0,64H160a8,8,0,0,0-8,8v56H104V160a8,8,0,0,0-8-8H40V104H96a8,8,0,0,0,8-8V40h48V96a8,8,0,0,0,8,8h56Z" />
    </g>
    <g v-else-if="weight === 'fill'">
      <path
        d="M232,108v40a16,16,0,0,1-16,16H164v52a16,16,0,0,1-16,16H108a16,16,0,0,1-16-16V164H40a16,16,0,0,1-16-16V108A16,16,0,0,1,40,92H92V40a16,16,0,0,1,16-16h40a16,16,0,0,1,16,16V92h52A16,16,0,0,1,232,108Z" />
    </g>
    <g v-else-if="weight === 'light'">
      <path
        d="M216,90H166V40a14,14,0,0,0-14-14H104A14,14,0,0,0,90,40V90H40a14,14,0,0,0-14,14v48a14,14,0,0,0,14,14H90v50a14,14,0,0,0,14,14h48a14,14,0,0,0,14-14V166h50a14,14,0,0,0,14-14V104A14,14,0,0,0,216,90Zm2,62a2,2,0,0,1-2,2H160a6,6,0,0,0-6,6v56a2,2,0,0,1-2,2H104a2,2,0,0,1-2-2V160a6,6,0,0,0-6-6H40a2,2,0,0,1-2-2V104a2,2,0,0,1,2-2H96a6,6,0,0,0,6-6V40a2,2,0,0,1,2-2h48a2,2,0,0,1,2,2V96a6,6,0,0,0,6,6h56a2,2,0,0,1,2,2Z" />
    </g>
    <g v-else-if="weight === 'regular'">
      <path
        d="M216,88H168V40a16,16,0,0,0-16-16H104A16,16,0,0,0,88,40V88H40a16,16,0,0,0-16,16v48a16,16,0,0,0,16,16H88v48a16,16,0,0,0,16,16h48a16,16,0,0,0,16-16V168h48a16,16,0,0,0,16-16V104A16,16,0,0,0,216,88Zm0,64H160a8,8,0,0,0-8,8v56H104V160a8,8,0,0,0-8-8H40V104H96a8,8,0,0,0,8-8V40h48V96a8,8,0,0,0,8,8h56Z" />
    </g>
    <g v-else-if="weight === 'thin'">
      <path
        d="M216,92H164V40a12,12,0,0,0-12-12H104A12,12,0,0,0,92,40V92H40a12,12,0,0,0-12,12v48a12,12,0,0,0,12,12H92v52a12,12,0,0,0,12,12h48a12,12,0,0,0,12-12V164h52a12,12,0,0,0,12-12V104A12,12,0,0,0,216,92Zm4,60a4,4,0,0,1-4,4H160a4,4,0,0,0-4,4v56a4,4,0,0,1-4,4H104a4,4,0,0,1-4-4V160a4,4,0,0,0-4-4H40a4,4,0,0,1-4-4V104a4,4,0,0,1,4-4H96a4,4,0,0,0,4-4V40a4,4,0,0,1,4-4h48a4,4,0,0,1,4,4V96a4,4,0,0,0,4,4h56a4,4,0,0,1,4,4Z" />
    </g>
  </svg>
</template>
