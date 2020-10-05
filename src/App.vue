<template>
  <ul>
    <learning-resources
      v-for="res in storedResources"
      :key="res.id"
      :title="res.title"
      :description="res.description"
      :link="res.link"
    ></learning-resources>
  </ul>
</template>

<script>
import LearningResources from './components/learning-resources/LearningResources.vue';
export default {
  components: {
    LearningResources
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
