<template>
  <div class="event-card">
    <h1>{{ event.name }}</h1>
    <p>{{ event.description }}</p>
    <pre>{{ event.date }}</pre>
  </div>
</template>

<script>
export default {
  name: 'EventCard',
  props: {
    event: Object
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.event-card {
  border: 1px solid #ccc;
  border-radius: 5px;
  padding: 1rem;
  display: inline-block;
  width: 500px;
  h1 {
    color: #41b883;
  }
}
</style>
