<script lang="ts">
export default {
  name: "App",
  components: {
    CoronaStatistics,
  },
};
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import CoronaStatistics from "./components/CoronaStatistics.vue";
</script>

<template>
  <CoronaStatistics />
</template>

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
