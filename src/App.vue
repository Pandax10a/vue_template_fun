<template>
  <div id="app">
    <template-fun></template-fun>
  </div>
</template>

<script>
import TemplateFun from '@/components/TemplateFun.vue';



export default {
 
  components: {
    TemplateFun
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
