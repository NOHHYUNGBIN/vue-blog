<script setup>
const props = defineProps({
  blogData: Array,
});
</script>

<template>
  <div v-for="data in blogData" :key="data.number">
    <h5 @click="$router.push(`/detail/${data.number}`)">{{ data.title }}</h5>
    <p>{{ data.date }}</p>
  </div>
</template>
