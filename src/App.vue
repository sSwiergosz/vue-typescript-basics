<template>
  <div class="app">
    <p>{{ name }} - {{ age }}</p>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';
import Job from './types/Job';

export default defineComponent({
  name: 'App',
  components: {},
  setup() {
    const jobs = ref<Job[]>([
      {
        title: 'Farm worker',
        location: 'Warsaw',
        salary: 1200,
        id: '1',
      },
      {
        title: 'Fisherman',
        location: 'Somewhere over the rainbow',
        salary: 1500,
        id: '2',
      }
    ])

    return { jobs }
  },
});
</script>

<style>
</style>
