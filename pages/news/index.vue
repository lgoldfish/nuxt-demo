<template>
  <div>
      <h2>News Index Page</h2>
      <p>newsId:{{$route.params.newsId}}</p>
      <span>{{newsId}}</span>
      <ul>
          <li><nuxt-link :to="{name:'index'}">Home</nuxt-link></li>
      </ul>
  </div>
</template>
<script>
    export default{
        transition:"test",
        data(){
            return {
                newsId:this.$route.params.newsId
            }
        }
    }
</script>

