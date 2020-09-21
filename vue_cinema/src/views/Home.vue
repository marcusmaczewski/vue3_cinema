<template>
  <div class="home">
    <Header msg="Welcome to Your Vue.js App"/>
    <Hero msg='VUE Bio'/>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import Hero from '@/components/Hero.vue'

import '@/components/style.css'


export default {
  name: 'Home',
  components: {
    Header,
    Hero
  }
}
</script>
