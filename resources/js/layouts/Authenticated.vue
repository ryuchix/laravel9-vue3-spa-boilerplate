<template>
  <main>
    <navigation></navigation>
    <div class="container mx-auto">
      <router-view></router-view>
      <div class="md:flex text-xs text-gray-500 py-8 px-2 md:px-0 break-words space-x-4">
        <span>© 2020 Ragnarok Mobile</span>
      </div>
    </div>
  </main>
</template>

<script>
import Navigation from '@/js/components/Navigation'

export default {
  components: {
    Navigation,
  },
  computed: {
    user() {
      return this.$store.getters.user
    }
  },
}
</script>
