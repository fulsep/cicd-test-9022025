<script setup lang="ts">

const nav = [
  { label: 'Home', to: '/' },
]
</script>

<template>
  <NuxtExample
    dir="routing/pages"
    :nav="nav"
    current-route
  >
    <NuxtLoadingIndicator />
    <NuxtPage />
  </NuxtExample>
</template>
