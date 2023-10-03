<template>
    <div>
        <p class="text-3xl mb-5">List available products</p>
        <div class="grid grid-cols-4 gap-5">
            <template v-for="p in products" :key="p.id">
                <ProductCard :product="p" />
            </template>
        </div>
    </div>
</template>

<script setup>
definePageMeta({

})
useHead({
    title: 'Nuxt Product Page',
    meta: [
        {name: 'product page', content: 'Product Page'}
    ]
})
const { data: products } = await useFetch('https://fakestoreapi.com/products')
</script>

<style lang="scss" scoped></style>