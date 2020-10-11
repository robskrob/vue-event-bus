<template>
  <div id="app" class="h-screen bg-orange-200 flex flex-col justify-center items-center">
    <component-a></component-a>
    <component-b></component-b>
  </div>
</template>

<script>

import ComponentA from './components/ComponentA'
import ComponentB from './components/ComponentB'

export default {
  name: 'App',
  components: {
    ComponentA,
    ComponentB,
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
