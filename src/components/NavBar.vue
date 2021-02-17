<template>
  <div class="">
    <div class="flex justify-between md:justify-around">
      <div>
        <img class="h-11  mt-4" src="../assets/logo.png" alt="someshit">
      </div>
      <div>
        <h1 class="mt-3 ml-2 font-bold text-4xl tracking-tighter text-purple-700">some real shit</h1>
      </div>
      <div>
        <button @click="isOpen = !isOpen" class="mt-6 ">
          <svg v-if="!isOpen" class="h-4" viewBox="0 0 18 15">
            <path fill="#6D28D9" d="M18,1.484c0,0.82-0.665,1.484-1.484,1.484H1.484C0.665,2.969,0,2.304,0,1.484l0,0C0,0.665,0.665,0,1.484,0 h15.031C17.335,0,18,0.665,18,1.484L18,1.484z"/>
            <path fill="#6D28D9" d="M18,7.516C18,8.335,17.335,9,16.516,9H1.484C0.665,9,0,8.335,0,7.516l0,0c0-0.82,0.665-1.484,1.484-1.484 h15.031C17.335,6.031,18,6.696,18,7.516L18,7.516z"/>
            <path fill="#6D28D9" d="M18,13.516C18,14.335,17.335,15,16.516,15H1.484C0.665,15,0,14.335,0,13.516l0,0 c0-0.82,0.665-1.484,1.484-1.484h15.031C17.335,12.031,18,12.696,18,13.516L18,13.516z"/>
          </svg>
          <svg v-if="isOpen" class="h-4" viewPort="0 0 12 12" version="1.1"
            xmlns="http://www.w3.org/2000/svg">
            <line x1="1" y1="20" 
                  x2="20" y2="1" 
                  stroke="#6D28D9" 
                  stroke-width="2"/>
            <line x1="1" y1="1" 
                  x2="20" y2="20" 
                  stroke="#6D28D9" 
                  stroke-width="2"/>
          </svg>
        </button>
      </div>
    </div>    
    <div :class="isOpen ? 'block' : 'hidden'" class="pt-4 md:mx-12">
      <a href="#" class="block px-2 py-1 text-purple-700 font-semibold rounded hover:bg-gray-100">Some link</a>
      <a href="#" class="mt-1 block px-2 py-1 text-purple-700 font-semibold rounded hover:bg-gray-100">Some shit</a>
      <a href="#" class="mt-1 block px-2 py-1 text-purple-700 font-semibold rounded hover:bg-gray-100">Some link</a>
      <a href="#" class="mt-1 block px-2 py-1 text-purple-700 font-semibold rounded hover:bg-gray-100">Some shit</a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NavBar',
  data() {
    return {
      isOpen: false,
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
