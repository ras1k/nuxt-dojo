<script setup>
const { id } = useRoute().params;
const uri = 'https://fakestoreapi.com/products/' + id ;

const { data: product } = await useFetch(uri, {key: id})
</script>

<template>
  <div>
    <p>{{ product.id }}</p>
    <img :src="product.image" alt="">
    <p>{{ product.title }}</p>
    <p>{{ product.price }}</p>
  </div>
</template>

<style lang="scss" scoped></style>
