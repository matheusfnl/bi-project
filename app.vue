<template>
  <div class="app-wrapper">
    <div class="sidebar">
      <SideBar />
    </div>

    <div class="app">
      <NuxtPage />
    </div>
  </div>
</template>

<style scoped>
  .app-wrapper {
    display: flex;
    height: 100vh;
    background-image: linear-gradient(to right top, #1f1d1e, #201a1f, #1f1821, #1c1624, #171527, #111628, #091628, #001728, #001824, #03191f, #0a191b, #111818);
  }

  .app {
    flex: 1;
    padding: 8px;
    max-width: 1440px;
    margin: 0 auto;
  }

  .page-enter-active,
  .page-leave-active {
    transition: all 0.4s;
  }
  .page-enter-from,
  .page-leave-to {
    opacity: 0;
    filter: blur(1rem);
  }
</style>