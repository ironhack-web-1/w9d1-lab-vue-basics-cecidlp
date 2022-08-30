<template>
  <div>
    <div v-for="project in projects" :key="project.name"> Items name {{project.name}}</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      projects: null,
    };
  },

  created() {
    fetch(
      "https://raw.githubusercontent.com/ironhack-jc/mid-term-api/main/projects"
    )
      .then((response) => response.json())
      .then((items) => (this.projects = items));
  },
};
</script>

<style></style>
