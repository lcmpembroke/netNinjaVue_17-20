<template>
  <div>
    <h1>{{ title }}</h1>

    <h2>{{ description }}</h2>

    <ninjas></ninjas>

  </div>
</template>

<script>
import Ninjas from './Ninjas.vue'

export default {
  components: {
    'ninjas': Ninjas
  },
  data () {
    return {
      title: 'Ninja App...',
      description: 'App.vue imports Ninjas.vue, and within the template of App.vue, uses the ninjas tag from import',
    }
  }
}
</script>

<style scoped>
h1 {
  color: purple
}

h2 {
  color: orangered
}

</style>
