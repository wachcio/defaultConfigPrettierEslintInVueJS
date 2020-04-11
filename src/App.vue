<template>
  <div id="app">
    <img
      v-if="true"
      alt="Vue logo"
      src="./assets/logo.png"
      title="hjghj"
    />
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
  mounted() {
    const newLocal = [2, 2, 2, 4];
    newLocal.push("4");
    console.log(`Hello ${newLocal}`);
    return { arr: newLocal };
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
