<script setup>
    import {defineProps} from "vue"

    const {name, url} = defineProps([
        'name',
        'url'
    ])
</script>

<template>
    <NCard title="Card with Cover">
        <template #cover>
            {{ url }}
        </template>
        <h3>{{ name }}</h3>
  </NCard>
</template>

<style scoped>
    .n-card {
        width: 200px;
        margin:10px 20px;
        height: 400px;

    }
    .n-card img {
        height: 250px
    }
</style>