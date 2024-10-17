<template>
  <header class="flex flex-col sm:flex-row justify-between items-center border-b border-slate-200 px-6 sm:px-10 py-4 sm:py-8">
    <!-- Логотип и информация -->
    <div class="flex items-center gap-4 mb-4 sm:mb-0">
      <img src="/jewelry-logo.png" alt="Logo" class="w-9 sm:w-11" />
      <div>
        <h2 class="font-bold text-lg sm:text-xl uppercase">Jewelry Store</h2>
        <p class="text-slate-400 text-sm sm:text-base">Лучший магазин бижютерии</p>
      </div>
    </div>

    <!-- Меню -->
    <ul class="flex flex-col sm:flex-row items-center gap-4 sm:gap-10">
      <li class="flex items-center gap-3 cursor-pointer">
        <img src="/cart.svg" alt="Cart" class="w-5 sm:w-auto" />
        <b class="text-sm sm:text-base">1205 грн.</b>
      </li>
      <li class="flex items-center gap-3 cursor-pointer">
        <img src="/heart.svg" alt="Favorite" class="w-5 sm:w-auto" />
        <span class="text-sm sm:text-base">Избранное</span>
      </li>
    </ul>
  </header>
</template>
