<script setup lang="ts">
import Autoplay from 'embla-carousel-autoplay'
import { Carousel, CarouselContent, CarouselItem } from '@/components/ui/carousel'

const plugin = Autoplay({
  delay: 1400,
  stopOnMouseEnter: true,
  stopOnInteraction: false
})
</script>

<template>
  <Carousel
    class="relative w-full max-w-2xl"
    :plugins="[plugin]"
    @mouseenter="plugin.stop"
    @mouseleave="[plugin.reset(), plugin.play(), console.log('Running')]"
  >
    <CarouselContent>
      <CarouselItem>
        <div class="flex flex-col items-center justify-center h-full">
          <div class="text-4xl font-bold text-primary px-14 text-center">
            Currently, 850 million people around the world are undernourished
          </div>
        </div>
      </CarouselItem>
      <CarouselItem>
        <div class="flex flex-col items-center justify-center h-full">
          <img src="@/assets/2-problem.png" alt="Problems" />
        </div>
      </CarouselItem>
    </CarouselContent>
  </Carousel>
</template>
