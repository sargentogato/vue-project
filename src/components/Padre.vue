<template>
  <div class="container">
    <h2>Soy el componente padre</h2>
    <div class="boxChild" v-for="value in values" v-bind:key="value.message">
      <child-component :messageFromFather="value" />
    </div>
  </div>
</template>

<script>
import childComponent from "./Hijo.vue";

export default {
  name: "fhaterComponent",
  components: {
    childComponent,
  },
  data: function () {
    return {
      values: [
        { message: "item 1", counter: 0 },
        { message: "item 2", counter: 0 },
        { message: "item 3", counter: 0 },
      ],
    };
  },
};
</script>

<style>
.boxChild {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  background-color: rgb(247, 247, 247);
}

h2 {
  flex-basis: 100%;
}
</style>
