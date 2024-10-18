<script setup>
defineProps({
  img: String,
  title: String,
  price: Number,
  onClickDelete: Function,
});
</script>

<template>
  <div class="relative flex w-full border border-slate-100 rounded-xl p-2 sm:p-4 gap-2 sm:gap-4">
    <img :src="img" class="w-16 h-16" alt="Jewelry" />
    <div class="flex flex-col w-full">
      <p class="text-sm sm:text-base lg:text-lg">{{ title }}</p>
      <div class="flex justify-between mt-2 sm:mt-5">
        <span class="font-bold text-sm sm:text-base lg:text-lg">{{ price }} грн.</span>
        <img
          @click="onClickDelete"
          class="cursor-pointer opacity-30 hover:opacity-100 transition w-4 sm:w-5 lg:w-6"
          src="/close.svg"
          alt="Close"
        />
      </div>
    </div>
  </div>
</template>
