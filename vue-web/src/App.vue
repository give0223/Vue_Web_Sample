<template>
  <div class="app">
    <Menu/>
    <div class="cover"></div>
    <div class="content">
      <router-view/>
    </div>
  </div>
</template>

<script>
import Menu from './Menu.vue';
export default {
  components:{
    Menu,
  }
}
</script>

<style>
  html,body,.app{
    padding:0;
    margin:0;
    color: #444;
  }
</style>

<style scoped>
  .cover{
    width: 100%;
    height:250px;
    background: url('./imgs/jill-heyer-247995-unsplash.jpg') center center no-repeat;
    background-size:cover;
  }
  .content{
    width:100%;
    padding:0 80px 80px;
    box-sizing: border-box;
  }
</style>
