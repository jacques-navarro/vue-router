<template>
  <h1>Jobs</h1>
  <div v-for="job in jobs">
    <router-link :to="{name: 'JobDetails', params: { id: job.id}}"
      >{{ job.title }} - {{ job.details }}</router-link
    >
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
