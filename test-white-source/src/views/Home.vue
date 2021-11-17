<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <div id="chartDom"></div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import echarts from 'echarts';

export default {
  name: "Home",
  components: {
    HelloWorld,
  },
  mounted(){
    echarts.init(document.getElementById(chartDom));
  }
};
</script>
