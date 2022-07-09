<template>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
  <DarkMode />
</template>

<script>
import DarkMode from './components/DarkMode.vue'

export default {
  name: 'App',
  components: {
    DarkMode,
  },
}
</script>

<style>
html.dark {
  color-scheme: dark;
  transition: color-scheme all 0.5ms;
}

body {
  @apply: bg-slate-50 text-slate-800 dark:bg-slate-800 dark:text-slate-50;
}
</style>
