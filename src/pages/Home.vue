<script setup>
import Card from '../components/Card.vue';
import Header from '../components/Header.vue';
</script>

<template>
  <div class="bg-white w-full sm:w-4/5 lg:w-3/5 xl:w-2/3 m-auto rounded-xl shadow-xl shadow-grey-200 mt-6 sm:mt-10 lg:mt-20">
    <Header />

    <div class="p-4 sm:p-6 lg:p-10">
      <div class="flex flex-col lg:flex-row justify-between items-center mb-6 lg:mb-10 gap-4">
        <h1 class="text-xl sm:text-2xl lg:text-3xl font-bold">Все товары</h1>
        <div class="flex flex-col sm:flex-row items-center gap-4 w-full sm:w-auto">
          <select
            class="py-2 px-3 border border-gray-200 focus:border-gray-400 rounded-md focus:outline-none w-full sm:w-auto"
          >
            <option value="name">По названию</option>
            <option value="price">По цене (дешевые)</option>
            <option value="price">По цене (дорогие)</option>
          </select>
          <div class="relative w-full sm:w-auto">
            <input
              type="text"
              class="w-full sm:w-auto border border-gray-200 rounded-md py-2 pl-10 pr-4 focus:outline-none focus:border-gray-400"
              placeholder="Поиск..."
            />
            <div class="absolute inset-y-0 left-0 pl-3 flex items-center pointer-events-none">
              <img src="/search.svg" />
            </div>
          </div>
        </div>
      </div>

      <!-- Адаптивная сетка карточек -->
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-4 sm:gap-6 lg:gap-10">
        <Card
          title="Печатка мужская с камнями"
          :price="120"
          img="/jewelry/jewelry-1.jpg"
        />
        <Card
          title="Брошь &quot;Панда&quot; лимонная позолота"
          :price="140"
          img="/jewelry/jewelry-2.jpg"
        />
        <Card
          title="Серьги классические &quot;Подкова&quot; лимонная позолота"
          :price="50"
          img="/jewelry/jewelry-3.jpg"
        />
        <Card
          title="Браслет &quot;Пересечения&quot; родий"
          :price="120"
          img="/jewelry/jewelry-4.jpg"
        />
        <Card
          title="Комплект &quot;Кассандра&quot; лимонная позолота"
          :price="130"
          img="/jewelry/jewelry-5.jpg"
        />
        <Card
          title="Цепочка с подвеской &quot;Капля росы&quot; позолота"
          :price="180"
          img="/jewelry/jewelry-6.jpg"
        />
        <Card
          title="Подвеска &quot;Череп&quot; сталь"
          :price="200"
          img="/jewelry/jewelry-7.jpg"
        />
        <Card
          title="Подвеска &quot;Биткоин&quot; сталь"
          :price="160"
          img="/jewelry/jewelry-8.jpg"
        />
        <Card
          title="Браслет широкий с черной керамикой"
          :price="600"
          img="/jewelry/jewelry-9.jpg"
        />
        <Card
          title="Браслет позолота двухрядное якорное плетение 0,3/19 см"
          :price="88"
          img="/jewelry/jewelry-10.jpg"
        />
        <Card
          title="Серьги-гвоздики &quot;Камень 0,3 см&quot; родий"
          :price="30"
          img="/jewelry/jewelry-11.jpg"
        />
        <Card
          title="Подвеска &quot;Кошечка&quot; лимонная позолота"
          :price="70"
          img="/jewelry/jewelry-12.jpg"
        />
      </div>
    </div>
  </div>
</template>
