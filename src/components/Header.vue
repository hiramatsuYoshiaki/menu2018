<template>
  <div class="header">
    <div id="nav">
      <router-link to="/" class="nav-items">2017</router-link> |
      <router-link to="/project" class="nav-items">2018</router-link>
      <!-- <router-link to="/collection">framework</router-link>|
      <router-link to="/about">about</router-link>|
      <router-link to="/contact">contact</router-link> -->
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.header{
  text-align: center;
  margin: 1rem;
}
.header #nav .nav-items{
  padding: 0 1rem;
}

 
</style>
