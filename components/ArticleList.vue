<template>
  <a href="#">
    <div class="grid mx-20 grid-cols-4 gap-5">
    <article
      v-for="article in articles"
      :key="article.id"
      class="border pb-3 bg-white border-opacity-20 border-black rounded-lg hover:scale-105 duration-300 ease-in-out"
    >
      <img :src="article.pict" class="rounded-t-lg border-b border-opacity-40 h-[200px] w-full object-cover" />
      <div class="px-3 mt-2">
        <h2 class="text-lg font-semibold">{{ article.title }}</h2>
        <div class="flex mt-1.5">
          <p class="font-normal text-sm">By {{ article.author }}</p>
          <p class="font-normal text-sm ml-auto">{{ article.date }}</p>
        </div>
      </div>
    </article>
  </div>
  </a>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'ArticleList',
  props: {
    articles: {
      type: Array,
      required: true
    }
  }
})
</script>
