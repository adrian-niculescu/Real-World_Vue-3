<template>
  <div class="events">
    <h1>Events for Good</h1>
    <img alt="Vue logo" src="../assets/logo.png" />
    <EventCard v-for="event in events" :key="event.id" :event="event"/>
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from "@/components/EventCard.vue";

export default {
  name: "Home",
  components: {
    EventCard
  },
  data() {
    return {
      events: [
      {
        id: 5928101,
        category: 'aimal welfare',
        title: 'Cat Adoption Day',
        description: 'Find your new feline friend',
        location: 'Meow Town',
        date: 'Jan 28, 2022',
        time: '12:00',
        petsAllowed: true,
        organizer: 'Kat Laydee'
      },
      {
        id: 5928102,
        category: 'food',
        title: 'Community Gardening',
        description: 'Find your new feline friend',
        location: 'Meow Town',
        date: 'Jan 28, 2022',
        time: '12:00',
        petsAllowed: true,
        organizer: 'Kat Laydee'
      },
            {
        id: 4828102,
        category: 'another',
        title: 'Community Gardening',
        description: 'Find your new feline friend',
        location: 'Meow Town',
        date: 'Jan 21, 2022',
        time: '12:00',
        petsAllowed: true,
        organizer: 'Kat Laydee'
      }
      ]
    }
  }
};
</script>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>