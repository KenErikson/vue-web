<template>
  <footer>
      <div class="top-border">
        <p class="color-primary-80">Made by me &copy; {{ year }} </p>
      </div>
  </footer>
</template>

<script>
import { computed } from 'vue'

export default {
  setup () {
    const year = computed(() => new Date().getFullYear())
    return { year }
  }
}
</script>
