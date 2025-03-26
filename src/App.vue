<script setup lang="ts">
import SiteNavbar from './components/SiteNavbar.vue';
import FrameComponent from './components/FrameComponent.vue'
import SpeedInsights  from "@vercel/speed-insights/vue"
</script>

<template>
  <SiteNavbar />
  <FrameComponent />
  <SpeedInsights />
</template>
