
<!-- Grid.vue -->
<script lang="ts">
export default {
  data() {
    const ROWS = 30
    const COLS = 30
    return {
      grid: Array.from({ length: ROWS }, () => Array(COLS).fill('')),
    };
  },
};
</script>

<template>

    <div class="grid">
      <div v-for="(row, rowIndex) in grid" :key="rowIndex" class="flex">
        <div
          v-for="(_, colIndex) in row"
          :key="colIndex"
          class="h-5 w-5 border border-gray-300"
        >
        </div>
      </div>
    </div>

  </template>

  <style scoped>

  </style>
