<script setup lang="ts">
import { ref } from "vue";

const props = defineProps<{
  initial?: number
}>()
const counter = ref(props.initial ?? 0)
</script>

<template>
  <slot name="top"></slot>
  <button @click="counter++">{{ counter }}</button>
  <slot name="bottom"></slot>
</template>

<style scoped></style>