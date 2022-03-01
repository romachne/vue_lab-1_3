<template>
  <div>
    <h1>Новости</h1>
    <all-news/>
  </div>
</template>

<script>
import { defineComponent } from 'vue'
import AllNews from '@/components/AllNews.vue'

export default defineComponent({
  name: 'NewsView',
  components: {
    AllNews
  }
})
</script>
