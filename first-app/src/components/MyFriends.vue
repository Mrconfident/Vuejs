<template>
  <li>
    <h2> {{friend.name}} </h2>
    <button @click="toggleDetails"> Show details</button>
    <ul v-if="isVisible">
      <li> <strong>Phone Number :</strong> {{ friend.phoneNo}}</li>
      <li> <strong>Email Address :</strong> {{ friend.email}} </li>
    </ul>
  </li>
  
</template>

<script>
export default {
  props: {
    friend: {
      type: Object,
      default: () => {},
      required: false
    }
  },
  data() {
    return {
      isVisible: false
    }
  },
  methods: {
    toggleDetails() {
      this.isVisible = !this.isVisible
    }
  }
}
</script>

<style scoped>

</style>