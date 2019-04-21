<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <div id="btn_ctr"></div>
    <div id="ipt_area">
      <div>
        <Viewedit v-model="article"></Viewedit>
      </div>
      <div>
        <textarea v-model="article" name="" id="" cols="30" rows="10"></textarea>
        
      </div>
    </div>
  </div>
</template>

<script>
import Viewedit from './components/Viewedit.vue'

export default {
  name: 'app',
  data(){
    return{
      article:"<a href='#'>hello</a>"
    }
  },
  components: {
    Viewedit
  }
}
</script>

<style>
#app {
  
}
</style>
