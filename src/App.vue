<script setup>
  import { useMonitor } from '@/composables/monitor';

  const { menu, footer } = useMonitor();
  
</script>

<template>
  <div>
    <component :is="menu" />
    
    
    <main>
      <router-view />
    </main>
    
  </div>
  <component :is="footer" />
</template>