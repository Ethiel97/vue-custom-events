<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld @changeMsg="setMessage" :msg="welcomeMsg"/>
  </div>
</template>

<script>
/* eslint-disable */

import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "app",
  data() {
    return {
      welcomeMsg: "Hello World"
    };
  },
  methods: {
    setMessage(msg) {
      this.welcomeMsg = msg;
    }
  },
  components: {
    HelloWorld
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
