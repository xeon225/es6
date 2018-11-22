<template>
  <div id="letConst">
    <div>
      let命令{{let()}}<br>
      {<br>
        var a = 10;<br>
        let b = 1;<br>
      }
    </div>
    
  </div>
</template>

<script>
import Vue from 'vue';


export default {
  name: 'Business',
  data () {
    return {

    }
  },
  mounted() {

  },
  methods: {
    let(){
      {
        var a = 10;
        let b = 1;
      }
      console.log(a);
      try{
        console.log(b);
        
      }catch(e){
        console.log('b is not defined');//sojson is undefined
      }
      for (let i = 0; i < 3; i++) {
        let i = 'abc';
        console.log(i);
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>


</style>
