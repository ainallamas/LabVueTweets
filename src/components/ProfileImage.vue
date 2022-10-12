<template>

<img class="imagen" :src="props.image" />

</template>

<script setup>

import {defineProps} from 'vue'

const props = defineProps (['image']);


</script>

<style scoped>

.imagen {
    height: 70px;
    margin: 5px 20px 0px 20px;
    border-radius: 50%;
}

</style>