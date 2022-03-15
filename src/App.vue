<template>
  <div id="app">
    <TheNavbar />
    <router-view />
  </div>
</template>
<script>
import TheNavbar from './components/TheNavbar.vue'
export default {
  components: { TheNavbar },
}
</script>
