<template>
    <div>
        <p>About</p>
        <p>{{ data.message }}</p>
    </div>
</template>

<script setup>
const { data } = await useFetch('/api/test?name=Bar', {
    method: 'post',
    body: {
        age: 25
    }
})
</script>

<style lang="scss" scoped></style>