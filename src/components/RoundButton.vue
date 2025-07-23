<template>
  <button
    type="button"
    :class="[
      'bg-gray-200 text-sm font-medium rounded-full px-3 py-1',
      variants[variant] ?? variants.default,
    ]"
    @click.prevent="$emit('click')"
  >
    <slot></slot>
  </button>
</template>

<script setup>
const variants = {
  default: 'border-gray-300 hover:bg-gray-100',
  danger: 'bg-red-200 enabled:hover:bg-red-100 text-red-900',
}

defineProps({
  variant: {
    type: String,
    default: 'default',
  },
})

defineEmits(['click'])
</script>
