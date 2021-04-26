<template>
  <div class="container">
    <h2>Soy el componente padre</h2>
    <child-component />
  </div>
</template>

<script>
import childComponent from "./Hijo.vue";

export default {
  name: "fhaterComponent",
  components: {
    childComponent,
  },
};
</script>

<style>
.container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  padding: 2rem 0;
  background-color: rgb(247, 247, 247);
}

h2 {
  flex-basis: 100%;
}
</style>
