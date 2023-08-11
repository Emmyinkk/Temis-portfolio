<template>
  <navbar />
  <router-view v-slot="{ Component }">
      <transition name="route" mode="out-in">
          <component :is="Component" :key="$route.path" />
      </transition>
  </router-view>
  <bottom-nav />
</template>

<script>
import navbar from './components/navbar.vue'
import bottomNav from './components/bottom-nav.vue'

export default {
  name: 'App',
  components: {
    navbar,
    bottomNav
  }
}
</script>

<style>
  .route-enter-from {
    opacity: 0;
    transform: translateX(100px);
  }
  .route-enter-active {
    transition: all 0.3s ease-out;
  }
  .route-leave-to {
    opacity: 0;
    transform: translateX(-100px);
  }
  .route-leave-active {
    transition: all 0.3s ease-in;
  }
</style>
