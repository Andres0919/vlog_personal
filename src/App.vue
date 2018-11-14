<template>
  <div id="app">
    <HelloWorld />
    <img id="background"  alt="">
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  }
}
</script>

<style>
*{
  margin: 0;
  color: #fff;
}

#app {
  background-image: linear-gradient(180deg, rgba(0, 0, 0, .15), rgba(0, 0, 0, .15)),url('./assets/background.jpg');
  background-position: 0px 0px, 50% 50%;
  background-size: 100%;
  position: absolute;
  width: 100%;
  height: 100%;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  text-align: center;
  color: #2c3e50;
}

#background{
  width: 50%; 
}
</style>
