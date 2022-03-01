<template>
  <div v-for="article in data" :key="article.id">
    <div>
      <h2>
        <router-link :to="{
          name: 'fullnews',
          params: {
            id: article.id,
            headline: article.headline,
            date: article.date,
            text: article.text
          }
        }">
          {{article.headline}}
        </router-link>
      </h2>
      <p>{{article.date}}</p>
      <p>{{article.text}}</p>
    </div>
  </div>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'AllNews',
  data () {
    return {
      data: []
    }
  },
  mounted () {
    const baseUrl = process.env.BASE_URL
    const jsonurl = (baseUrl + 'server/articles.json')
    fetch(jsonurl)
      .then(response => response.json())
      .then(data => { this.data = data })
  }
})
</script>
