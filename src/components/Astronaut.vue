<script setup lang="ts">
import { useMouse } from '@vueuse/core';
const { x, y } = useMouse()

</script>

<template>
    <span id="rotateMe">🧑‍🚀 {{ x }}  {{ y }}</span>
</template>

<style scoped>
#rotateMe {
    transform-origin: center center;
    transition: transform 0.1s
}
</style>