<template>
  <div>
    <h1>{{ msg }}</h1>
    <Area />
  </div>
</template>

<script>
  import Area from 'arc_charts';

  export default {
    name: 'app',
    components: {
      Area,
    },
    data () {
      return {
        msg: 'Welcome to Your Vue.js App'
      }
    }
  }
</script>
