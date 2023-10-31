<script setup lang="ts">
    import { ref } from 'vue'
    import ECompeteView from '@/views/ECompeteView.vue';
    import HomeView from '@/views/AboutView.vue';
    import AboutViewVue from '@/views/AboutView.vue';

    const isOpen = ref(true)

</script>

<template>
    <div class="menuContainer">
        <button v-on:click="isOpen=!isOpen" value="value setting" title="title setting">
            <img alt="toggle menu" class="menu" src="@/assets/menu.jpg" width="32" height="32" />
        </button>
       <!-- <div v-if="isOpen">open menu</div>
        <div v-else> closed menu</div>
       -->
        <div v-show="isOpen">
          <nav>
            <RouterLink to="/">Home</RouterLink>
            <RouterLink to="/ECompete">eCompete</RouterLink>
            <RouterLink to="/about">About</RouterLink>
          </nav>
        </div>
        <div v-show="!isOpen"></div>

     `<div>{{ isOpen }}</div>`
    </div>
  </template>

<style scoped>


@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>