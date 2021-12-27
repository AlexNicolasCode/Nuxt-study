<template>
  <div>
    <h1>Continent: {{ continent }}</h1>
    <h2>Mountain: {{ title }}</h2>
    <p>Path: {{ $route.path }}</p>
    <NuxtLink to="/">Back to Mountains</NuxtLink>
  </div>
</template>
<script>
export default {
  async asyncData({ params, error, payload }) {
    if (payload) return { title: payload.title }
  }
}
</script>
