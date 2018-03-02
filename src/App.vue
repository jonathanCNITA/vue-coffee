<template>
  <div id="app">
    <h1>{{ msg }}</h1>
    <img src="./assets/coffee_icon.png">
    <app-buttons></app-buttons> 
  </div>  
</template>

<script>
import Buttons from './Buttons.vue';
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome Vue Coffee App',
      
    }
  },
  components: {
    'app-buttons': Buttons
  }
}
</script>

<style lang="scss">
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

.all-buttons {
  margin-top: 20px;
  margin-bottom: 20px;
}
</style>
