<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
// import storage from './storage'

export default {
  name: 'App',
  components: {
   
  },
  data(){
    return {
      res:{}

    }
  },
  mounted(){
    // storage.setItem('a',1);
    // storage.setItem('a',1,'user');
    // storage.clear('mall');
    this.axios.get('/mock/user/login.json').then((res)=>{
      this.res = res;
    });
  }
}
</script>

<style>

</style>
