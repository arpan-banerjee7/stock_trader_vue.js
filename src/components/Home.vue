<template>
  <div>
    <h1>Trade or View your Portfolio</h1>
    <h4>You may Save & Load your Data</h4>
    <h4>Click on 'End Day' to begin a New Day!</h4>
    <hr />
    <p>Your Funds : {{ funds | currency }}</p>
  </div>
</template>

<script>
export default {
  computed: {
    funds() {
      return this.$store.getters.funds;
    },
  },
};
</script>

<style scoped>
h1 {
  font-family: "Lato", cursive, sans-serif;
}

p {
  font-family: "Ranchers", cursive, sans-serif;
  font-size: 150%;
  color: rgba(0, 0, 0, 0.774);
}
</style>