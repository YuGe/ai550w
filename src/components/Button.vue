<template>
  <button
    :class="[
      'rounded-xl font-medium transition',
      size === 'lg' ? 'px-6 py-3 text-base' : 'px-4 py-2',
      variant === 'outline'
        ? 'border border-slate-600 text-slate-200 hover:bg-slate-800'
        : 'bg-indigo-500 text-white hover:bg-indigo-400',
    ]"
  >
    <slot />
  </button>
</template>

<script setup lang="ts">
defineProps<{
  variant?: "default" | "outline";
  size?: "md" | "lg";
}>();
</script>
