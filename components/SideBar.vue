<template>
  <div class="sidebar-wrapper">
    <NuxtLink :to="item.path" :class="{ 'checked' : isChecked(item) }" class="sidebar-item" v-for="(item, index) in items" :key="index">
      <component :is="item.icon" />
    </NuxtLink>
  </div>
</template>

<script setup>
  import { shallowRef } from 'vue';

  import IconAbout from './icons/About.vue';
  import IconHome from './icons/Home.vue'
  import IconGraph from './icons/Graph.vue';

  const route = useRoute()
  const isChecked = (item) => {
    console.log(route)
  }

  const items = shallowRef([
    {
      icon: IconHome,
      path: '/'
    },
    {
      icon: IconAbout,
      path: '/about'
    },
    {
      icon: IconGraph,
      path: '/project'
    },
  ]);
</script>

<style scoped>
  .sidebar-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    height: 100%;
    padding: 8px;
    background-color: rgba(255, 255, 255, 0.10);
    gap: 4px;
  }

  .sidebar-item {
    padding: 4px;
    aspect-ratio: 1/1;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 6px;
    cursor: pointer;
    transition: .2s all;
    color: white;
  }

  .sidebar-item:hover {
    background-color: rgba(25, 250, 220, 0.2);
    color: white;
  }

  .sidebar-item.checked {
    background-color: rgba(25, 250, 220, 0.2);
    color: white;
  }
</style>