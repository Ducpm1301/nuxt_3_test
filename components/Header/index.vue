<template>
    <nav class="container mx-auto p-4 flex justify-between">
        <nuxt-link to="/">Nuxt</nuxt-link>
        <ul class="flex gap-4">
            <li>
                <nuxt-link to="/home">Home</nuxt-link>
            </li>
            <li>
                <nuxt-link to="/about">About</nuxt-link>
            </li>
            <li>
                <nuxt-link to="/product" class="btn">Products</nuxt-link>
            </li>
        </ul>
    </nav>
</template>

<script setup>

</script>

<style scoped>
.router-link-exact-active {
    color:#12b488;
}

</style>