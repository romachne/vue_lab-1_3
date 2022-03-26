<template>
  <div>
    <div>
      <h2>{{$route.params.name}}</h2>
      <p>{{$route.params.date}}</p>
      <p>{{$route.params.desc}}</p>
    </div>
  </div>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'FullNews'
})
</script>
