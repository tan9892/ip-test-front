<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <HelloWorld msg=""/>
    <SECTION />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import SECTION from '@/views/section/section.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    SECTION
  }
}
</script>
