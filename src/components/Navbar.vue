<script setup lang="ts">
import { isDark, toggleDark } from '~/composables'
</script>

<template>
  <nav class="text-xl p-5 flex justify-between">
    <button class="icon-btn !outline-none font-bold">
      <div i-carbon-menu />
    </button>

    <button class="icon-btn !outline-none font-bold" @click="toggleDark()">
      <div v-if="isDark" i-carbon-moon />
      <div v-else i-carbon-sun />
    </button>
  </nav>
</template>
