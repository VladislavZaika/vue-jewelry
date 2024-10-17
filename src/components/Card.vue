<script setup>
import { ref } from 'vue';

defineProps({
  title: String,
  img: String,
  price: Number,
});

const isLiked = ref(false);

const onClick = () => {
  isLiked.value = !isLiked.value;
};
</script>

<template>
  <div
    class="relative flex flex-col w-full border border-slate-100 rounded-xl p-4 sm:p-6 lg:p-8 cursor-pointer transition hover:shadow-xl hover:transform hover:-translate-y-2"
  >
    <div @click="onClick" class="absolute top-4 sm:top-6 left-4 sm:left-6">
      <img :src="isLiked ? '/like-2.svg' : '/like-1.svg'" alt="Favorite" class="w-5 sm:w-6 lg:w-8" />
    </div>
    <img :src="img" class="w-full h-auto object-cover" alt="Sneaker" />
    <p class="text-sm sm:text-base lg:text-lg mt-4">{{ title }}</p>
    <div class="flex justify-between mt-3 sm:mt-5">
      <div class="flex flex-col gap-1 sm:gap-2">
        <span class="text-slate-200 text-xs sm:text-sm">Цена:</span>
        <span class="font-bold text-sm sm:text-base lg:text-lg">{{ price }} грн.</span>
      </div>
      <img src="/plus.svg" alt="Plus" class="w-5 sm:w-6 lg:w-8" />
    </div>
  </div>
</template>
