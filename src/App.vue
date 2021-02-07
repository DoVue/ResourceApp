<template>
  <ResourceItem msg="Welcome to Your Vue.js App"/>
  <ul></ul>
</template>

<script>
import ResourceItem from './components/learning-resources/ResourceItem';

export default {
  name: 'App',
  components: {
    ResourceItem
  },
  data() {
    return {
      storedResources: [
        {
          id: 'official-guide',
          title: 'Official Guide',
          description: 'The official VueJS documentation',
          link: 'https://vuejs.org/v2/guide/'
        },
        {
          id: 'google',
          title: 'Google',
          description: 'Learn to Google...',
          link: 'https://google.org'
        }
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
