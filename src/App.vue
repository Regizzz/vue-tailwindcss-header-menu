<template>
  <div class="px-8 py-2 max-w-md mx-auto sm:max-w-xl lg:max-w-full">
    <NavBar class="z-10" />
    <MainShit class="z-0"/>
  </div>
  
</template>

<script>
import NavBar from './components/NavBar.vue'
import MainShit from './components/MainShit.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    MainShit
  }
}
</script>

<style>

</style>
