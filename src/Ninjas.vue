<template>
<div>
  <h2>List of Ninjas using v-for to perform looping through ninjas data array</h2>
  <ul>
    <li v-for="(ninja,index) in ninjas" v-bind:key="index">{{ index + 1 }} {{ ninja }}</li>
   </ul>
  </div>
</template>

<script>
  export default {
      data() {
          return {
              ninjas: ['Ninja1 cool name', 'Ninja2 strong name', 'Ninja3 mighty name']
          }
      },
  }

</script>

<style scoped>
h2 {
  color: green
}

</style>
