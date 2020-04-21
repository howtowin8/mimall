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
    // 本地加载请求静态json文件的形式
    this.axios.get('/user/login').then((res)=>{
      this.res = res;
    });
  }
}
</script>

<style>

</style>
