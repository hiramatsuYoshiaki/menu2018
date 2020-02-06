<template>
  <div class="home">
    <HomeContent msg="2017 Develop Menu"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import HomeContent from '@/components/HomeContent.vue'

export default {
  name: 'home',
  components: {
    Header,
    HomeContent
  }
}
</script>
