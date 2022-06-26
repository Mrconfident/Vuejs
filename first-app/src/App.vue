<template>
  <h2> My friends </h2>
  <ul>
    <my-friends v-for="friend in friends" :key="friend.id" :friend="friend"/>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      friends: [
        {
          id: 'Vikas',
          name: 'Vikas yadav',
          phoneNo: 9089897777,
          email: 'x@gmail.com',
        },
        {
          id: 'Tarun',
          name: 'Tarun Jain',
          phoneNo: 9089898877,
          email: 'x@gmail.com',
        }
      ]
    }
  }
}
</script>

<style>
</style>
