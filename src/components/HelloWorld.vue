<script lang="ts">
import axios, { AxiosResponse } from 'axios'

let a : AxiosResponse<any, any>;
export default {
  name: 'HelloWorld',
  data() {

    return {
      statistics : a
    }
  },
  mounted() {
    axios
    .get('https://coronavirusapifr.herokuapp.com/data/live/france')
    .then((response) => {
      this.statistics = response;
      console.log(this.statistics)
    })
  }
}
</script>

<template>
<h1> Date </h1>
</template>

<style scoped>

</style>
