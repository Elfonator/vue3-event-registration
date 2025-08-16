<template>
  <SectionCard>
    <div class="flex justify-between">
      <div>{{ title }}</div>
      <RoundButton variant="danger" @click="$emit('cancel')"> Cancel </RoundButton>
    </div>
  </SectionCard>
</template>

<script setup>
import SectionCard from '@/components/SectionCard.vue';
import RoundButton from '@/components/RoundButton.vue';
defineProps({
  title: String,
});
defineEmits(['cancel']);
</script>
