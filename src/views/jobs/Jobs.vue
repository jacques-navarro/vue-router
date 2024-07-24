<template>
  <h1>Jobs</h1>
  <div v-for="job in jobs">
    <span>{{ job.title }} - {{ job.details }}</span>
  </div>
</template>

<script>
export default {
  data() {
    return {
      jobs: [
        { title: "UX Designer", id: 1, details: "blah" },
        { title: "Web Developer", id: 2, details: "blah" },
        { title: "Vue Developer", id: 3, details: "blah" },
      ],
    };
  },
};
</script>

<style></style>
