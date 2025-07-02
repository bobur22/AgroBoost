<script setup lang="ts">
import SolutionsCard from '@/components/SolutionsCard.vue'
</script>

<template>
  <div class="flex flex-col gap-8 items-center m-2 rounded-xl h-[150vh] bg-[#E1EAF9]">
    <p class="text-4xl my-12 text-primary">We are here to solve them</p>

    <SolutionsCard
      class="w-3/4"
      title="Accurate diagnosis"
      body="We provide accurate diagnosis for the diseases that plants are facing using drones. We use AI to analyze the data collected by drones."
    >
      <template #pic>
        <img src="@/assets/2-problem.png" alt="Solutions" />
      </template>
    </SolutionsCard>
  </div>
</template>

<style scoped></style>
