<template>
  <div id="app">
    <img src="./assets/logo.png">
    <h1>{{ msg }}</h1>
    <button type="button" class="btn btn-primary btn-lg" v-on:click="toggle">Chart Click!!!</button>
    <span v-show="isOpen"><Chart></Chart></span>
  </div>
</template>

<script>
import Chart from './Chart.vue'
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      isOpen: false
    }
  },
  components: {
    Chart
  },
  methods: {
    toggle: function(){
      this.isOpen = !this.isOpen
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
