<script setup lang="ts">
import RoundedCard from '@/components/RoundedCard.vue'
</script>

<template>
  <RoundedCard class="animate-pulse">
    <div class="p-4 border b border-gray-200 h-6 bg-gray-300"></div>
    <div class="p-4 border b border-gray-200 h-4 bg-gray-300"></div>
    <div class="p-4 h-4 bg-gray-300"></div>

    <div class="flex justify-end p-4">
      <div class="h-8 w-24 bg-gray-300 rounded-full"></div>
    </div>
  </RoundedCard>
</template>
