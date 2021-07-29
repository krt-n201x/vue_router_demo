<template>
  <div v-if="event">
    <h1>{{ event.name }}</h1>
    <p>Trips : {{ event.trips }}</p>
  </div>
</template>
<script>
export default {
  props: ['event'],
  computed: {
    checkid: function () {
      var id = this.event._id
      if (id == '5f1c59d0fa523c3aa793c0ac') {
        return true
      } else return false
    }
  }
}
</script>
<style scoped>
img {
  height: 50px;
}
</style>
