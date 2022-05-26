<template>
  <div class="app">
    <JobsList :jobs="jobs"/>
  </div>
</template>

<script setup lang="ts">
import type Job from "./types/Job";
import { ref } from "vue";
import JobsList from "./components/JobsList.vue";

const jobs = ref<Job[]>([
  {
    title: "farm worker",
    location: "lon lon ranch",
    salary: 30000,
    id: 1,
  },
  {
    title: "Warrior",
    location: "basement",
    salary: 5000,
    id: 2,
  },
]);
</script>

<style>
</style>

