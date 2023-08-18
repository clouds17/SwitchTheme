<template>
    <div :class="{ [baseClassName]: true }">
      <slot v-if="$slots.default"></slot>
    </div>
  </template>
  
  <script setup lang="ts">
  import { prefixName } from '@/assets/theme/index';
  const baseClassName = `${prefixName}-box`;
  </script>