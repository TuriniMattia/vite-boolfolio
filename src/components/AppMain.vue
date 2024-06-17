<template>
  <div>
    <h2>Progetti</h2>
  </div>
</template>

<script>
import axios from 'axios';
export default {


  data() {


    return {
      projects: [],
    }
  },
  methods: {
    fetchProjects() {
      axios.get('http://127.0.0.1:8000/api/projects')
    },
  },
  created() {
    this.fetchProjects();
  },


}
</script>

<style lang="scss" scoped></style>
