<template>
    <div class="card text-center">
        <img :src="product.image" alt="Product thumb" class="thumb">
        <p class="font-bold text-gray-500 m-4 truncate">{{ product.title }}</p>
        <nuxt-link :to="`/product/${product.id}`">
            <p class="btn">View detail</p>
        </nuxt-link>
    </div>
</template>

<script setup>
const { product } = defineProps([
    'product'
])
</script>

<style scoped>
    .thumb {
        max-height: 120px;
        max-width: 70%;
        margin: 0 auto;
    }
</style>