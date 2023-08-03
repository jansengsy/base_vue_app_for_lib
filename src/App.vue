<template>
  <div>
    <h1>{{ msg }}</h1>
    <div class="wrapper">
      <!-- <Test class="box"/> -->
      <Area class="box"/>
      <Area class="box"/>
      <Area class="box"/>
      <Area class="box"/>
    </div>
  </div>
</template>

<script>
  import Area from 'arc_charts';
  import Test from './components/Test.vue';

  export default {
    name: 'app',
    components: {
      Area,
      Test,
    },
    data () {
      return {
        msg: 'Welcome to the Vue.js App'
      }
    }
  }
</script>

<style>
  .flex-container {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    width: 100%;
    height: 100vh;
    margin: 5px;
  }

  .flex-item {
    flex: 1;
    height: 400px;
    background-color: #ddd;
    border: 1px solid #888;
    padding: 5px;
  }

  .wrapper {
    display: grid;
    width: 100%;
    grid-template-columns: 33% 33% 33%;
    grid-gap: 10px;
    background-color: #fff;
    color: #444;
  }

  .box {
    background-color: #888;
    color: #fff;
    height: 380px;
    border-radius: 5px;
    padding: 10px;
    font-size: 150%;
  }

</style>