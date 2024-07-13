<template>
    <nav class="bg-[#361173] text-white ">
      <NuxtLink to="/" class="hover:font-bold text-lg font-medium pl-20">Beranda</NuxtLink>
      <NuxtLink to="/about" class="hover:font-bold text-lg font-medium pl-5">Tentang</NuxtLink>
    </nav>
  </template>
  
  <script>
  import { defineComponent } from 'vue'
  
  export default defineComponent({
    name: 'Navigation'
  })
  </script>
  
  <style scoped>
  nav {
    padding: 1rem 0;
  }
  a {
    margin-right: 1rem;
  }
  </style>