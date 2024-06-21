<template>
  <div>
    <h2>Progetti</h2>
    <ProjectCard />
  </div>
</template>

<script>
import axios from 'axios';
import ProjectCard from 'ProjectCard.vue';
export default {


  data() {
    components: {
      ProjectCard,
    },
    return {
      projects: [],
    }
  },
  methods: {
    fetchProjects() {
      axios.get('http://127.0.0.1:8000/api/projects').then(res => {
        console.log(res.data.results.data)
        this.projects = res.data.results.data
      })
    }
  },
  created() {
    this.fetchProjects();
  },


}
</script>

<style lang="scss" scoped></style>
