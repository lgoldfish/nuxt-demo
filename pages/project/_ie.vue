<template>
  <div>
      <h2>project-content:{{$route.params}}</h2>
    <ul>
        <li>
            <nuxt-link to="/">Home</nuxt-link>
        </li>
    </ul>
  </div>
</template>
<script>
export default {
  data(){
      return {
          title:this.$route.params.title
      }
  },
  head(){
      return {
          title:this.title,
          meta:[
              {hid:'description',name:'project',content:'this is a project '}
          ]
      }
  }
}
</script>

