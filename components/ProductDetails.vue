<template>
    <div class="card">
        <div class="flex flex-col md:grid md:grid-cols-2 md:gap-10">
            <div class="">
                <img :src="`${product.image}`" class="mx-auto my-7 max-w-[200px] lg:max-w-[400px]" />
            </div>
            <div class="">
                <h2 class="text-4xl my-7">{{ product.title }}</h2>
                <p class="text-xl my-7">Price - ${{ product.price }}</p>
                <h3 class="font-bold border-b-2 mb-4 pb-2">Product description:</h3>
                <p class="mb-7">{{ product.description }}</p>
            </div>
        </div>
    </div>
</template>
  
<script setup>
const { product } = defineProps(['product'])
</script>
  
<style scoped></style>