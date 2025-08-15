<template>
  <main class="mx-auto max-w-screen-xl my-8 space-y-8 px-4">
    <h1 class="text-4xl">Event Booking App</h1>
    <h2 class="text-2xl font-medium">All Events</h2>
    <section class="grid grid-cols-2 gap-8">
      <EventCard
        v-for="i in 8"
        :key="i"
        title="Vue Conference 2024"
        @register="console.log('Registered!')"
      />
    </section>
    <h2 class="text-2xl font-medium">Your Bookings</h2>
    <section class="grid grid-cols-1 gap-4">
      <BookingItem v-for="i in 3" :key="i"></BookingItem>
    </section>
  </main>
</template>

<script setup>
import EventCard from '@/components/EventCard.vue';
import BookingItem from '@/components/BookingItem.vue';
</script>
