<template>
  <div id="app">
    <img width="25%" src="./assets/logo.png">
    <HelloWorld :message="message"/>
    <button @click="ChangeMessage()">Change Message</button>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",
  components: {
    HelloWorld
  },
  data() {
    return {
      message: {
        message: "Welcome to Vue"
      }
    };
  },
  methods: {
    ChangeMessage() {
      this.message.message = "Message changed";
    }
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
