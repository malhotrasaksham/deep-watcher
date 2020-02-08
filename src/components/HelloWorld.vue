<template>
  <div class="hello">
    <h1>{{ message.message }}</h1>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    message: Object
  },
  watch: {
    message: {
      handler(to, from) {
        console.log("changed");
      },
      deep: true
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
