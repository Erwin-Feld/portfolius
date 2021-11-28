<template>
  <section class="p-5 bg-dark">
    <div class="container">
      <h2 class="text-center mb-4">My Projects</h2>

      <div class="row g-4">
        <project-card
          v-for="project in projectsJson"
          :image_src="require(`@/assets/images/${project.imgName}`)"
          :project_name="project.name"
          :key="project.name" 
        />
      </div>
    </div>
  </section>
</template>

<script>
import projectsJson from "../assets/comp.Data/projects.json";
import ProjectCard from "./ProjectCard.vue";



export default {
  components: { ProjectCard },
  name: "ProjectSection",

  setup() {
    return {
      projectsJson,
    };
  },
};
</script>
