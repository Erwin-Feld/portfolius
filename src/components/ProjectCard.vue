<template>
  <div class="col-md-6 col-lg-3">
    <div class="card bg-light">
      <div class="card-body text-center">
        <img :src="image_src" alt="" class="card-img-top mb-1" />
        <h3 class="card-title mb-1">{{ project_name }}</h3>
        <p class="card-text mb-1">it does some stuff</p>
        <p class="card-text mb-1">it does some stuff</p>
        <p class="card-text mb-1">it does some stuff</p>

        <!-- Add install boostrap icons in node -->
        <!-- <a href="#"><i class="bi bi-globe text-dark mx-1"></i></a> -->
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProjectCard",
  // props: [""],
  props: {
    image_src: {
      type: String,
      //  required: true,
    },

    project_name: {
      type: String,
    },
  },

  // setup(props) {

  // },
};
</script>
