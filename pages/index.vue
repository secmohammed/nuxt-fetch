<template>
  <div class="container">
    <User id="1" />
  </div>
</template>

<script>
import Vue from 'vue'
import User  from '@/components/User'
export default {
  components: {
    User
  },
  // data() {
  //   return {
  //     user: null
  //   }
  // },
  // async asyncData({ $axios }) {
  //   let user = await $axios.$get('https://jsonplaceholder.typicode.com/users/1')
  //   return { user}
  // }
}
</script>

<style>
</style>
