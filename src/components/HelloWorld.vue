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
    .then((response) => this.statistics = response.data)
  }
}
</script>

<template>
<h1> Date </h1>
<div v-for="(statistic,index) in statistics" :key="index">
  <p> {{statistic.date}} </p>
  <p> {{statistic.date ? statistic.date : null}} </p>
  
</div>
</template>

<style scoped>

</style>
