<template>
  <div class="home">    
    <Sidebar/>
    <Carousel/>
    <Modals/>
  </div>
</template>
<script>
// @ is an alias to /src
import Carousel from '@/components/Carousel.vue'
import Sidebar from '@/components/Sidebar.vue'
import Modals from '@/components/Modals.vue'

export default {
  name: 'Home',
  components: {
    Carousel,
    Sidebar,
    Modals
  }
}
</script>
