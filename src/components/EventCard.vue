<template>
  <router-link
    class="event-link"
    :to="{ name: 'event-show', params: { id: 1 } }"
  >
    <div class="event-card -shadow">
      <span class="eyebrow">@{{ event.time }} on {{ event.date }}</span>
      <h4 class="title">{{ event.title }}</h4>
      <span>{{ event.attendees.length }} attending</span>
    </div></router-link
  >
</template>

<script>
export default {
  data() {
    return {
      event: {
        id: 1,
        title: 'Park Cleanup',
        date: 'Tues Nov 3, 2021',
        time: '6:00',
        attendees: [
          {
            id: 'serhan01',
            name: 'Serhan Elmalı',
          },
          {
            id: 'lopers',
            name: 'Lorem Person',
          },
        ],
      },
    }
  },
}
</script>

<style scoped></style>
