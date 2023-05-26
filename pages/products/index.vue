<template>
  <div>
    <h1 class="flex justify-center text-center mb-4 text-xl font-semibold">All Products</h1>
    <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-5">
      <div v-for="product in products" :key="product.id">
        <ProductCard :product="product" />
      </div>
    </div>
  </div>
</template>

<script setup>
definePageMeta({
  layout: 'products'
});

// fetch all products
const { data: products } = await useFetch('https://fakestoreapi.com/products')
</script>

<style lang="scss" scoped></style>
