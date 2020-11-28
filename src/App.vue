<template>
  <div id="app">
    <Watch/>
    <Calculator/>
  </div>
</template>

<script>
import Watch from './components/Watch.vue';
import Calculator from './components/Calculator.vue';

export default {
  name: 'App',
  components: {
    Watch,
    Calculator,
  },
};
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
