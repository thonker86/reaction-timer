<template>
  <p>Your Reaction Time is {{ score }} ms ({{ rank }})</p>
</template>

<script>
export default {
  props: ["score"],
  computed: {
    rank() {
      return this.score > 250 ? "Train More" : "Rapid Reflexs";
    },
  },
};
</script>

<style>
</style>