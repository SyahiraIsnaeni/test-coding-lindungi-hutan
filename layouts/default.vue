<template>
  <div class="bg-[#E1EDF3] h-full">
    <Navigation />
    <slot />
  </div>
</template>

<script setup>
import Navigation from '~/components/Navigation.vue'
</script>