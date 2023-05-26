<template>
  <div>
    <h2>Product Detail</h2>
    <p>id from route param: {{ id }}</p>
  </div>
</template>

<script setup>
const { id } = useRoute().params;
definePageMeta({
  layout: 'products'
})
</script>

<style lang="scss" scoped></style>
