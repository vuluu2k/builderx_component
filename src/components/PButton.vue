<script setup lang="ts">
import AButton from "ant-design-vue/es/button";

defineProps({
});


</script>

<template>
  <AButton v-bind="$attrs">
    <slot></slot>
  </AButton>
</template>
