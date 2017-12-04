<template>
  <div id="app">
    <HelloWorld/>
    <Test></Test>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import Test from './components/Test'

export default {
  name: 'app',
  components: {
    HelloWorld,
    Test
  }
}
</script>

<style>
#app {
}
</style>
