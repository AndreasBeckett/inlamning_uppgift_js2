<template>
  <div>
    <navbar />
    <div class="container mt-4">
      <router-view/>
    </div>
    
  </div>
</template>

<script>
import Navbar from './components/Navbar/Nav'
export default {
  components:{
    Navbar
  }

}
</script>

<style>

</style>
