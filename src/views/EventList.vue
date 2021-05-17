<template>
  <div class="event">
    <img alt="Vue logo" src="../assets/logo.png" />
    <h1>Titre EventCard</h1>
    <EventCard v-for="event in events" :key="event.id" :event="event" />
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
        id:5929001,
        category: 'animal welfare',
        title: 'Cat Adoption Day', 
        description: 'find your new feline',
        location: 'MEow Town',
        date: 'January 28, 2022',
        time: '12:00',
        petsAllowed:true,
        organizer: 'Kat Laydee'
        },
        {
        id:5929002,
        category: 'animal welfare',
        title: 'Cat Adoption Day', 
        description: 'find your new feline',
        location: 'MEow Town',
        date: 'January 28, 2022',
        time: '12:00',
        petsAllowed:true,
        organizer: 'Kat Laydee'
        }, 
        {
        id:5929003,
        category: 'animal welfare',
        title: 'Cat Adoption Day', 
        description: 'find your new feline',
        location: 'MEow Town',
        date: 'January 28, 2022',
        time: '12:00',
        petsAllowed:true,
        organizer: 'Kat Laydee'
        } 
       ] 
    }
  }

};
</script>

<style scoped>
.events
{
display:flex;
flex-direction:column;
align-items:center;
}
</style>
