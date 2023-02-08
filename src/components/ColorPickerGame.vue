<template>
  <h1>Color Picker Game</h1>

  <div>{{ message }}</div>

  <button v-for="color in colors" :key="color" @click="matchColor(color)">
    {{ color }}
  </button>
</template>

<script>
import { colorDetector } from "../composables/colorDetector";
export default {
  setup() {
    return colorDetector();
  },
};
</script>

<style></style>
