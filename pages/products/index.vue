<template>
  <div>
    <h1>Products</h1>
    <div class="grid grid-cols-4 gap-5">
      <div v-for="p in products">
        <NuxtLink :to="`/products/${p.id}`">{{ p.title }}</NuxtLink>
        <img :src='p.image' alt="">
      </div>
    </div>
  </div>
</template>

<script setup>
const { data: products } = await useFetch('https://fakestoreapi.com/products')
</script>

<style lang="scss" scoped>

</style>