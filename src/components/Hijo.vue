<template>
  <div>
    <div class="box">
      <p>{{ messageFromFather.message }}</p>
      <button class="btn" v-on:click="count(messageFromFather)">
        {{ messageFromFather.counter }}
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "childComponent",
  props: ["messageFromFather"],
  methods: {
    count(value) {
      value.counter++;
    },
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
