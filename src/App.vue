<template>
  <div id="app">
    <div v-for="item in urlDatas"><a :href="item.url" v-text="item.title"></a></div>
  </div>
</template>

<script>
import urlData from './assets/urlD.json';
export default {
  name: 'App',
  data () {
    return {
      msg: {
      },
    }
  },
  computed:{
    urlDatas(){
      return urlData.datas;
    }
  },
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
