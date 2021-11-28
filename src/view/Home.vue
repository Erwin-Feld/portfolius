<template>
  <nav-bar />
  <project-section />
</template>

<script>
import NavBar from "../components/NavBar.vue";
import ProjectSection from "../components/ProjectSection.vue";

export default {
  name: "Home",
  components: {
    NavBar,
    ProjectSection,
  },
};
</script>
