<template>
  <div id="app" class="container" >

   <h1>Vue Js</h1>

  <Post>
    <h2 slot="cabecalho" >Components no vue</h2>
    
    <p class="post-paragrafo" >Components são importantes no vue</p>
    <span>...</span>
  
    <small slot="rodape" >por {{autor}} </small>    
  </Post>



  </div>
</template>

<script>

import  Post  from './components/Post'

export default {
  components: {
    Post
  },
  data(){
    return{
      autor: 'Arduino'
    }
  }
}
</script>

<style scoped>
  .container{
    width: 960px;
    margin: auto;
  }

 
</style>
