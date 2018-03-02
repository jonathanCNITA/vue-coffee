<template>
  <div id="app">
    <h1>{{ msg }}</h1>
    <img src="./assets/coffee_icon.png">
    <img src="">
    <div class="all-buttons" v-for="machine in machines">
      <label for="bt">MASCHINE {{ machine.id }}</label>
      <toggle-button name="bt" v-model="machine.state"/>
    </div>
  </div>  
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome Vue Coffee App',
      machines: [
        {id: 1, state: true},
        {id: 2, state: false},
        {id: 3, state: true},
        {id: 4, state: false},
        {id: 5, state: false},
        {id: 6, state: false}
      ]
    }
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
