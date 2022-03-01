<template>
  <div>
    <div>
      <h2>{{$route.params.headline}}</h2>
      <p>{{$route.params.date}}</p>
      <p>{{$route.params.text}}</p>
    </div>
  </div>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'FullNews'
})
</script>
