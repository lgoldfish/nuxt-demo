<template>
  <div>
      <h2>News-Content [{{$route.params.id}}]</h2>
     <span>{{$route.params}}</span>
      <ul>
        <li><a href="/">Home</a></li>
      </ul>
  </div>
</template>
<script>
export default {
  validate ({params}){
      console.log("params id",params)
     return /^\d+$/.test(params.id)
  }
}
</script>