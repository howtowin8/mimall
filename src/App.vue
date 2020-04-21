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
  mounted(){
    // storage.setItem('a',1);
    // storage.setItem('a',1,'user');
    // storage.clear('mall');
  }
}
</script>

<style>

</style>
