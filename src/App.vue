<template>
  <h1>{{ message }}</h1>
  <AppMain />
  <ProjectCard />
</template>

<script>
import AppMain from './components/AppMain.vue';
import ProjectCard from './components/ProjectCard.vue'
export default {
  components: {
    AppMain,
    ProjectCard,
  },
  data() {


    return {
      message: 'ciao mondo',
    }
  }
}
</script>

<style lang="scss" scoped></style>