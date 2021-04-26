<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <fhater-component />
  </div>
</template>

<script>
import fhaterComponent from "./components/Padre.vue";

export default {
  name: "App",
  components: {
    fhaterComponent,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
