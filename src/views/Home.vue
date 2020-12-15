<template>
  <div class="home">
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from '@/components/EventCard.vue'

export default {
  name: 'Home',
  components: {
    EventCard
  },
  data() {
    return {
      events: [
        {
          id: 1,
          name: 'Aprender Vue en VueMastery',
          date: '5-12-2020',
          description: 'Apender Real Word Vue antes de finalizar Diciembre'
        },
        {
          id: 2,
          name: 'Hacer ejercicio',
          date: '01-01-2021',
          description: 'New Year resolution'
        },
        {
          id: 3,
          name: 'Comer mejor',
          date: '01-01-2021',
          description: 'New Year resolution'
        }
      ]
    }
  }
}
</script>

<style lang="scss">
.home {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>