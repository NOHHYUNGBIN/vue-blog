<script setup>
const props = defineProps({
  blogData: Array,
});
</script>

<template>
  <div>
    <h4>상세페이지</h4>
    <h5>{{ blogData[$route.params.id].title }}</h5>
    <p>{{ blogData[$route.params.id].content }}</p>
  </div>
</template>
