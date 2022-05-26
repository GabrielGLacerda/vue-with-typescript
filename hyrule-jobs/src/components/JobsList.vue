<template>
  <div>
    <ul>
      <li v-for="job in jobs" :key="job.id" >
        <h2>{{ job.title }} in {{ job.location }}</h2>
        <div class="salary">
          <p>{{ job.salary }} rupees</p>
        </div>
        <div class="description">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Rem ab non quia ad, quasi odio veniam quas molestias amet voluptates, eum sint, cupiditate quis labore obcaecati voluptas ratione soluta magni.
        </div>
      </li>
    </ul>
  </div>
</template>

<script setup lang="ts">
import type Job from '@/types/Job'
// import type { PropType } from 'vue';
// const jobs = defineProps({
//   jobs: {
//     required: true,
//     type: Array as PropType<Job[]>
//   }
// })

const jobs = defineProps<{
  jobs: Array<Job>
}>()
</script>

<style scoped>
</style>