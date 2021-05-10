<template>
  <h1 v-if="num === 5">Hello</h1>
  <h1 v-else-if="num > 0">номер</h1>
  <h1 v-else-if="num < 0">-номер</h1>
  <h1 v-else>Не номер</h1>

  <template v-if="display">
    <h1>Zhakshylyk</h1>
  </template>
  <h2 v-show="show">Use v-show</h2>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      num: 4,
      display: true,
      show: true
    };
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
