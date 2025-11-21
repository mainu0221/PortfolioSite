<template>
  <button
    @click="goTop"
    class="fixed bottom-8 right-8 bg-emerald-600 text-white w-12 h-12 rounded-full shadow-lg flex items-center justify-center hover:bg-emerald-700 transition z-50"
  >
    ^
  </button>
</template>

<script setup>
const goTop = () => {
  window.scrollTo({ top: 0, behavior: 'smooth' })
}
</script>
