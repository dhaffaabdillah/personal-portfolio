<template>
  <div class="container-page">
    <PreloaderComponents/>
    <HeaderComponents/>
    <router-view/>
    <FooterComponents/>
  </div>
  
  
</template>

<script>
import PreloaderComponents from './components/PreloaderComponents.vue'
import HeaderComponents from './components/HeaderComponents.vue'
import FooterComponents from './components/FooterComponents.vue'
import { inject } from '@vercel/analytics';
inject();
export default {
  name: 'App',
  components: {
    PreloaderComponents,
    HeaderComponents,
    FooterComponents,
  }
}
</script>
