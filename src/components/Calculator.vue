<template>
    <div id="calc">
        <div><input type="text" v-model='x' /> </div>
        <div><input type="text" v-model='y' /> </div>
        <div><span v-text='result'></span></div>
    </div>
</template>

<script>
function isNotNumber(value) {
  return Number.isNaN(value);
}
export default {
  name: 'Calculator',
  data() {
    return {
      x: 0,
      y: 0,
      lastResult: 0,
    };
  },
  computed: {
    result() {
      if (isNotNumber(this.x)) return this.lastResult;
      if (isNotNumber(this.y)) return this.lastResult;
      return `Результат сложения ${+this.x + +this.y}`;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
