<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps<{
  title: string
  body: string
}>()
</script>

<template>
  <div class="flex flex-row gap-2 items-center m-2 rounded-xl bg-[#E1EAF9]">
    <div class="flex flex-col items-center justify-center m-2 w-1/2">
      <p class="text-5xl my-4 text-primary">{{ props.title }}</p>
      <p class="text-3xl my-4 text-primary">{{ props.body }}</p>
    </div>

    <div class="flex flex-col gap-8 items-center m-2 rounded-xl bg-[#E1EAF9] w-1/2">
      <slot name="pic" />
    </div>
  </div>
</template>

<style scoped></style>
