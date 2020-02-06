<template>
  <div class="project">
    <ProjectContent msg="2018 Develop Menu"/>
  </div>
</template>
<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import ProjectContent from '@/components/ProjectContent.vue'

export default {
  name: 'home',
  components: {
    Header,
    ProjectContent
  }
}
</script>