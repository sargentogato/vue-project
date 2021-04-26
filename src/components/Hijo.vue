<template>
  <div>
    <div class="box" v-for="value in values" v-bind:key="value.message">
      <p>{{ value.message }}</p>
      <button class="btn" @click="value.counter++">{{ value.counter }}</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "childComponent",
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
.box {
  margin-block-end: 1rem;
  border: #0ed40e 3px solid;
}
.box {
  flex-basis: 100%;
  padding: 0.5rem 7rem;
}

.btn {
  color: white;
  padding: 0.2rem 0.8rem;
  background-color: #0ed40e;
}
</style>
