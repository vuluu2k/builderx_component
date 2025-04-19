<script setup lang="ts">
import AButton from "ant-design-vue/es/button";

defineProps({
  label: {
    type: String,
    default: "",
  },
  size: {
    type: String,
    default: "md",
  },
});
</script>

<template>
  <AButton v-bind="$attrs" :class="['p-btn', size]">
    <slot>{{ label }}</slot>
  </AButton>
</template>

<style>
@import url('./button.scss');
</style>