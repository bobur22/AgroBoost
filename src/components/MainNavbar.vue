<template>
  <div
    class="absolute font-extrabold z-10 p-5 main-navbar flex w-full text-xl text-primary justify-between px-5"
  >
    <div class="flex items-center">
      <div class="flex items-center gap-x-3"><IconTooling />eco</div>
      <ul>
        <li>Home</li>
        <li>Opportunities</li>
        <li>Contact</li>
      </ul>
    </div>

    <div class="flex items-center gap-x-3">
      <Button size="sm">Log In</Button>
      <Button size="sm" class="border-2" variant="secondary">Sign Up</Button>
    </div>
  </div>
</template>

<style scoped>
.main-navbar {
  font-family: 'DejaVu Sans Mono', monospace;
}

ul {
  margin-left: 4rem;
  display: flex;
  gap: 1rem;
  justify-content: space-around;
  list-style: none;
  padding: 0;
}

li {
  cursor: pointer;
}
</style>
<script setup lang="ts">
import IconTooling from '@/components/icons/IconTooling.vue'
import { Button } from '@/components/ui/button'
</script>
