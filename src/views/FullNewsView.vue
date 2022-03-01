<template>
  <div>
    <h1>Новость</h1>
    <full-news/>
  </div>
</template>

<script>
import { defineComponent } from 'vue'
import FullNews from '@/components/FullNews.vue'

export default defineComponent({
  name: 'FullNewsView',
  components: {
    FullNews
  }
})
</script>
