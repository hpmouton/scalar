/* GENERATED FILE */
<script lang="ts">
export default {
  name: 'ScalarIconGoodreadsLogo',
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
        d="M184,20a12,12,0,0,0-12,12v4.22A67.94,67.94,0,0,0,60,88v24a67.94,67.94,0,0,0,112,51.78V168a44.05,44.05,0,0,1-44,44c-15,0-30.29-7.58-38.16-18.87a12,12,0,0,0-19.68,13.74C82.5,224.56,105.21,236,128,236a68.07,68.07,0,0,0,68-68V32A12,12,0,0,0,184,20ZM128,156a44.05,44.05,0,0,1-44-44V88a44,44,0,0,1,88,0v24A44.05,44.05,0,0,1,128,156Z" />
    </g>
    <g v-else-if="weight === 'duotone'">
      <path
        d="M184,88v24a56,56,0,0,1-112,0V88a56,56,0,0,1,112,0Z"
        opacity="0.2" />
      <path
        d="M184,24a8,8,0,0,0-8,8V45.74A64,64,0,0,0,64,88v24a64,64,0,0,0,112,42.26V168a48.05,48.05,0,0,1-48,48c-16.45,0-32.72-8.08-41.44-20.58a8,8,0,1,0-13.12,9.16C85.06,221.24,106.48,232,128,232a64.07,64.07,0,0,0,64-64V32A8,8,0,0,0,184,24ZM128,160a48.05,48.05,0,0,1-48-48V88a48,48,0,0,1,96,0v24A48.05,48.05,0,0,1,128,160Z" />
    </g>
    <g v-else-if="weight === 'fill'">
      <path
        d="M200,24H56A16,16,0,0,0,40,40V216a16,16,0,0,0,16,16H200a16,16,0,0,0,16-16V40A16,16,0,0,0,200,24ZM176,160a48,48,0,0,1-86.4,28.8,8,8,0,1,1,12.8-9.6A32,32,0,0,0,160,160V147.74A48,48,0,0,1,80,112v-8a48,48,0,0,1,80-35.74V64a8,8,0,0,1,16,0Zm-16-56v8a32,32,0,0,1-64,0v-8a32,32,0,0,1,64,0Z" />
    </g>
    <g v-else-if="weight === 'light'">
      <path
        d="M184,26a6,6,0,0,0-6,6V51.4A62,62,0,0,0,66,88v24a62,62,0,0,0,112,36.6V168a50.06,50.06,0,0,1-50,50c-17.09,0-34-8.41-43.08-21.43a6,6,0,1,0-9.84,6.86C86.34,219.57,107.11,230,128,230a62.07,62.07,0,0,0,62-62V32A6,6,0,0,0,184,26ZM128,162a50.06,50.06,0,0,1-50-50V88a50,50,0,0,1,100,0v24A50.06,50.06,0,0,1,128,162Z" />
    </g>
    <g v-else-if="weight === 'regular'">
      <path
        d="M184,24a8,8,0,0,0-8,8V45.74A64,64,0,0,0,64,88v24a64,64,0,0,0,112,42.26V168a48.05,48.05,0,0,1-48,48c-16.45,0-32.72-8.08-41.44-20.58a8,8,0,1,0-13.12,9.16C85.06,221.24,106.48,232,128,232a64.07,64.07,0,0,0,64-64V32A8,8,0,0,0,184,24ZM128,160a48.05,48.05,0,0,1-48-48V88a48,48,0,0,1,96,0v24A48.05,48.05,0,0,1,128,160Z" />
    </g>
    <g v-else-if="weight === 'thin'">
      <path
        d="M184,28a4,4,0,0,0-4,4V58.13A60,60,0,0,0,68,88v24a60,60,0,0,0,112,29.87V168a52.06,52.06,0,0,1-52,52c-17.72,0-35.28-8.75-44.72-22.29a4,4,0,0,0-6.56,4.58C87.61,217.91,107.74,228,128,228a60.07,60.07,0,0,0,60-60V32A4,4,0,0,0,184,28ZM128,164a52.06,52.06,0,0,1-52-52V88a52,52,0,0,1,104,0v24A52.06,52.06,0,0,1,128,164Z" />
    </g>
  </svg>
</template>
