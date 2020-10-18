<template>
  <div id="app">
    <div id="nav">
      <router-link to="/" class="nav-link" >首页</router-link> 
      <router-link to="/AddBlog" title="添加" class="add"  >
        <img src="/add.png" alt="添加" >
      </router-link>
      <div class="Intr">
        <Introduction></Introduction>
      </div>
      <div class="Cal">
        <Calendarmodel />
      </div>
    </div>

    <router-view/>

  </div>
</template>



<script>
  import Introduction from "./components/Introduction";
  import Calendarmodel from "./components/Calendarmodel";
  export default {
    name: 'App',
    components: {
      Introduction,
      Calendarmodel
    }
  }
</script>

<style >
  #app{
    margin: 0;
    padding: 0;
    background:pink
    /*background: rgba(181,152,161,1);*/
  }
  #nav{
    background: black;
    height: 40px;
    padding: 10px 20px 10px 20px;
    margin: 0 auto;
    font-size: 2em;
    color: black;
    font-family: 黑体;
    position: sticky;
    top: 0;

  }
  #nav a{
    color: white;
    text-decoration: none;
  }
  /*.nav-link:hover{*/
  /*  font-size: 35px;*/
  /*}*/
  .add{
    float: right;
  }
  img{
    padding-top: 3px;
    width: 35px;
  }
  /*img:hover{*/
  /*  width: 37px;*/
  /*}*/
  @media screen and (max-width:1490px) {
    .Cal,.Intr {
      display: none;
    }
  }
  .Cal{
    position: static;
    margin-left: 10px;
    margin-top: 50px;
    float: right;
    font-size: 15px;
    padding: 0px;
    height: 100px;
  }
  .Cal button{
    display: none;
  }

</style>

