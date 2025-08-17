<template>
  <main class="mx-auto max-w-screen-xl my-8 space-y-8 px-4">
    <h1 class="text-4xl">Event Booking App</h1>
    <h2 class="text-2xl font-medium">All Events</h2>
    <EventList />
    <h2 class="text-2xl font-medium">Your Bookings</h2>
    <BookingList />
  </main>
</template>

<script setup>
import EventList from '@/components/EventList.vue';
import BookingList from './components/BookingList.vue';
</script>
