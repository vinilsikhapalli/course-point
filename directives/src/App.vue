<template>
  <div id="app">
    <h1>custom directives</h1>
   <custom-button></custom-button>
   <!-- <appFilter message="from the data passing through props passing "></appFilter> -->
   <app-filter></app-filter>
   <auto-populate-filter></auto-populate-filter>
  </div>
</template>

<script>
import customButton from './components/customButton.vue'
import  appFilter  from "./components/appFilter.vue";
import  autoPopulateFilter from "./components/autoPopulateFilter.vue";
export default {
  name: 'App',
  components: {
    customButton,
    appFilter,
    autoPopulateFilter
  }
}
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
