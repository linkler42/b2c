<script setup>
const categories = [
  'Все акции',
  'OLED телевизоры',
  'Iphone 14',
  'Samsung S23',
  'Ноутбуки',
  'Кондиционеры',
  'Стиральные машины',
  'Гарантия низкой цены',
  'PlayStation 5',
  'Умные колонки',
  'Пылесосы Dyson',
  'Тренажоры'
]
</script>

<template>
  <header class="flex flex-col mt-8 mx-auto w-full max-w-[1920px] h-[100px] px-4 lg:px-8">
    <div class="flex flex-wrap items-start gap-x-4 gap-y-4">
      <img src="/logo.svg" alt="Логотип магазина" class="w-[100px] md:w-auto" />
      <div class="leading-none flex flex-col justify-center">
        <p class="font-circe font-normal text-[18px] leading-[20px] m-0">itl.b2c</p>
        <p class="font-circe font-normal text-[14px] leading-[18px] m-0">Готовый интернет магазин</p>
      </div>
      <button class="flex items-center justify-center gap-2 w-[181px] h-[48px] px-5 py-3 rounded-md bg-[#FFD740] ml-0 md:ml-4">
        <img src="/humburger.svg" class="w-5 h-5" />
        <span class="font-circe font-normal text-[16px] text-center whitespace-nowrap">Каталог товаров</span>
      </button>
      <div class="relative flex-grow max-w-full md:max-w-[970px] h-[48px]">
        <input
          type="text"
          placeholder="Искать товар co скидками до 50%"
          class="w-full h-full border border-[#0E6CDD] border-opacity-0 border-2
                focus:border-opacity-100 focus:outline-none rounded-md
                pr-11 px-4 text-[16px] leading-6 font-circe transition-all duration-200"
        />
        <img src="/search.svg" alt="Поиск" class="absolute right-4 top-1/2 -translate-y-1/2 w-5 h-5" />
      </div>
      <div class="flex flex-wrap justify-between items-center w-full max-w-[400px] mt-2 gap-4">
        <div class="flex items-center gap-3 font-circe font-normal cursor-pointer">
          <img src="/profile.svg" alt="Войти" />Войти
        </div>
        <div class="flex items-center gap-3 font-circe font-normal cursor-pointer">
          <img src="/heart.svg" alt="Избранное" />Избранное
        </div>
        <div class="flex items-center gap-3 font-circe font-normal cursor-pointer">
          <img src="/basket.svg" alt="Корзина" />954 870
        </div>
      </div>
    </div>

    <nav class="flex justify-between flex-wrap gap-3 mt-3 font-circe font-normal text-[16px] text-blue-900">
      <NuxtLink
        v-for="(category, index) in categories"
        :key="index"
        to="#"
        class="hover:underline whitespace-nowrap">
        {{ category }}
      </NuxtLink>
    </nav>
  </header>

  <div class="">
    <slot />
  </div>

  <footer class="px-4 lg:px-8 mb-10">
    <div class="flex flex-col md:flex-row bg-[#0E6CDD0D] mx-auto w-full max-w-[1920px] h-auto md:h-[110px] rounded-md p-4 md:p-6 gap-4 md:gap-0">
      <div class="flex flex-col justify-center">
        <p class="font-circe font-normal text-[20px] leading-[18px] m-0 mb-2">Подпишитесь на нашу рассылку</p>
        <p class="font-circe font-normal text-[14px] leading-[18px] m-0">
          Вы первыми будите узнавать о наших акциях и эксклюзивных предложениях
        </p>
      </div>
      <div class="flex-grow md:ml-6 flex items-center">
        <input
          type="email"
          placeholder="Укажите ваш email"
          class="px-4 py-3 text-[#005CCC] bg-white focus:border-opacity-100 focus:outline-none focus:border-[#005CCC] w-full h-[52px] rounded-md border border-gray-300"
        />
        <button class="ml-4 bg-[#FFD740] rounded-md w-[150px] h-[52px] font-circe font-normal text-[16px] leading-[24px] text-center">
          Подписаться
        </button>
      </div>
    </div>

    <div class="flex flex-col md:flex-row justify-between mx-auto w-full max-w-[1920px] h-auto md:h-[220px] px-4 mt-16 gap-10 md:gap-0">
      <!-- Левая колонка -->
      <div class="flex flex-col max-w-[320px]">
        <div class="flex items-center mb-2">
          <p class="text-[30px]">+7 727 339 70 10</p>
          <img src="/downArrow.svg" class="w-5 ml-2" />
        </div>
        <p class="text-[#7D7D7D] font-circe text-[16px] font-normal leading-[24px] mb-4">
          Задать вопрос или оформить покупку
        </p>

        <div class="flex gap-5 mb-4">
          <div class="w-[45px] h-[45px] bg-[#0E6CDD0D] rounded-md flex items-center justify-center">
            <img src="/inst.svg" />
          </div>
          <div class="w-[45px] h-[45px] bg-[#0E6CDD0D] rounded-md flex items-center justify-center">
            <img src="/tg.svg" />
          </div>
          <div class="w-[45px] h-[45px] bg-[#0E6CDD0D] rounded-md flex items-center justify-center">
            <img src="/facebook.svg" />
          </div>
        </div>

        <NuxtLink to="#" class="font-circe font-normal text-[14px] leading-[24px] mb-1 hover:underline">
          Политика конфиденциальности
        </NuxtLink>
        <NuxtLink to="#" class="font-circe font-normal text-[14px] leading-[24px] hover:underline">
          Пользовательское соглашение
        </NuxtLink>
      </div>

      <div class="flex flex-wrap gap-10 md:gap-16">
        <!-- Магазин -->
        <div>
          <p class="font-circe font-normal text-[20px] text-[#333333] mb-2">Магазин</p>
          <p class="font-circe font-normal text-[16px] text-[#333333] mt-2">г. Алмата, ул. Толе Би 100</p>
          <p class="font-circe font-normal text-[14px] text-[#7D7D7D]">Открыто до 19:00</p>
          <p class="font-circe font-normal text-[16px] text-[#333333] mt-2">г. Алмата, ул. Пушкина 189</p>
          <p class="font-circe font-normal text-[14px] text-[#7D7D7D]">Открыто до 19:00</p>
          <p class="font-circe font-normal text-[16px] text-[#333333] mt-2">г. Алмата, ул. Фурманова 45</p>
          <p class="font-circe font-normal text-[14px] text-[#7D7D7D]">Открыто до 19:00</p>
        </div>

        <!-- О компании -->
        <div>
          <p class="font-circe font-normal text-[20px] text-[#333333] mb-3">О компании</p>
          <NuxtLink to="#" class="block font-circe font-normal text-[16px] text-[#333333] hover:underline mb-2">Акции и новости</NuxtLink>
          <NuxtLink to="#" class="block font-circe font-normal text-[16px] text-[#333333] hover:underline mb-2">Корпоративным клиентам</NuxtLink>
          <NuxtLink to="#" class="block font-circe font-normal text-[16px] text-[#333333] hover:underline mb-2">Вакансии</NuxtLink>
          <NuxtLink to="#" class="block font-circe font-normal text-[16px] text-[#333333] hover:underline mb-2">Контакты</NuxtLink>
          <NuxtLink to="#" class="block font-circe font-normal text-[16px] text-[#333333] hover:underline">Обратная связь</NuxtLink>
        </div>

        <!-- Помощь -->
        <div>
          <p class="font-circe font-normal text-[20px] text-[#333333] mb-3">Помощь</p>
          <NuxtLink to="#" class="block font-circe font-normal text-[16px] text-[#333333] hover:underline mb-2">Где мой заказ?</NuxtLink>
          <NuxtLink to="#" class="block font-circe font-normal text-[16px] text-[#333333] hover:underline mb-2">Обмен и возврат</NuxtLink>
          <NuxtLink to="#" class="block font-circe font-normal text-[16px] text-[#333333] hover:underline mb-2">Гарантии</NuxtLink>
          <NuxtLink to="#" class="block font-circe font-normal text-[16px] text-[#333333] hover:underline mb-2">Сервисные центры</NuxtLink>
          <NuxtLink to="#" class="block font-circe font-normal text-[16px] text-[#333333] hover:underline">Бонусные программы</NuxtLink>
        </div>

        <!-- Получение и оплата -->
        <div>
          <p class="font-circe font-normal text-[20px] text-[#333333] mb-3">Получение и оплата</p>
          <NuxtLink to="#" class="block font-circe font-normal text-[16px] text-[#333333] hover:underline mb-2">Доставка курьером</NuxtLink>
          <NuxtLink to="#" class="block font-circe font-normal text-[16px] text-[#333333] hover:underline mb-2">Доставка транспортной компанией</NuxtLink>
          <NuxtLink to="#" class="block font-circe font-normal text-[16px] text-[#333333] hover:underline mb-2">Самовывоз</NuxtLink>
          <NuxtLink to="#" class="block font-circe font-normal text-[16px] text-[#333333] hover:underline">Способы оплаты</NuxtLink>
        </div>
      </div>
    </div>

    <div class="w-full px-[18px] mt-10">
      <div class="w-full h-[1px] bg-[#DCEEFF]"></div>
    </div>

    <div class="flex flex-col md:flex-row justify-between items-center w-full max-w-[1920px] mx-auto mt-6 px-4 gap-4">
      <p class="font-circe font-normal text-[14px]">© ITL.B2C 2023</p>
      <img src="/Logo.New.svg" alt="Логотип ITL.B2C" />
    </div>
  </footer>
</template>
