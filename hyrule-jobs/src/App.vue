<script setup lang="ts">
import { ref } from 'vue'
  const name = ref('Link')
  const age = ref(30)
  const weapon = ref('sword')
</script>

<template>
  <div class="app">
    {{name}} - {{age}} - {{weapon}}
  </div>
</template>

<style>
</style>

