<template>
  <div>
      <h1>姓名：{{info.name}}</h1>
      <h1>age：{{info.age}}</h1>
      <h1>love：{{info.interest}}</h1>
      <ul>
          <li>
              <nuxt-link to="/">HOME</nuxt-link>
          </li>
      </ul>
  </div>
</template>
<script>
import axios from 'axios'
export default {
  data(){
      return {
          name:"hello async"
      }
  },
  async asyncData(){
      let {data} = await axios.get("https://api.myjson.com/bins/dacqz")
      return {info:data}
  }
}
</script>

