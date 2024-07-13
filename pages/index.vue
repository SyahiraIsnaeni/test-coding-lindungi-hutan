<template>
    <div class="mt-12">
      <h1 class="text-3xl text-center font-bold mb-10">Daftar Artikel</h1>
      <ArticleList :articles="articles" />
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  import ArticleList from '~/components/ArticleList.vue'
  
  const { data: articlesData } = await useFetch('https://mocki.io/v1/f93066fa-8321-4abf-8fa6-7db071f06994')
  const articles = ref(articlesData.value.articles)
  </script>