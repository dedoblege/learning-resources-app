<template>
  <ul>
    <stored-resources :resources="storedResources"></stored-resources>
  </ul>
</template>

<script>
import StoredResources from './components/learning-resources/StoredResources.vue';
export default {
  components: {
    StoredResources
  },
  data() {
    return {
      storedResources: [
        {
          id: 'offcial-guide',
          title: 'Official guide',
          description: 'The Official Vue.js documentation',
          link: 'http://vuejs.org'
        },
        {
          id: 'google',
          title: 'Google',
          description: 'Google knows everything',
          link: 'http://google.com'
        }
      ]
    };
  }
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'Roboto', sans-serif;
}

body {
  margin: 0;
}
</style>
