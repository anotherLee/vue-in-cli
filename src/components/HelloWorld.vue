<template>
  <div class="hello">
  </div>
</template>

<script>
import bus from '../../static/js/bus'
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  mounted () {
    bus.$on('test', function (msg) {
      alert('Hello ' + msg)
    })
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
