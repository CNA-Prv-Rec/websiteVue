<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<template>
  <div class="title">
    <h1 class="orange nowrap">{{ msg }}</h1>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  
}

h3 {
  font-size: 1.2rem;
}

.title h1,
.title h3 {
  text-align: center;
  
}
.nowrap {
  flex-wrap: nowrap;
}

@media (min-width: 1024px) {
  .title h1,
  .title h3 {
    text-align: left;
    
  }
}
</style>
