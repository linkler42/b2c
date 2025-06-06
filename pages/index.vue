<template>
  <div class="w-full max-w-[1920px] bg-[#F1F6FD] mb-[25px] px-4 lg:px-8 mx-auto">
    <section class="flex flex-col py-10 px-4 lg:px-8">
      <!-- Слайдеры -->
      <div class="flex gap-6 justify-center max-w-[1680px] mx-auto mb-6">
        <Swiper
          :slides-per-view="1"
          :loop="true"
          class="w-[1200px] h-[320px] overflow-hiden"
        >
          <SwiperSlide v-for="n in 3" :key="'first-' + n">
            <div class="relative w-full h-full flex items-center justify-center text-2xl font-bold bg-gray-200 rounded-xl">
              <img src="/public/baners/sliderBaner1.svg" class="w-full h-full object-cover rounded-[6px]"/>
              <p class="absolute bottom-[175px] left-[55px] font-circe font-normal text-[30px] self-start">
                Скидки до 50% на вотрой товар <br> встраиваемой техники.
              </p>
              <p class="absolute bottom-[100px] left-[55px] font-circe font-normal text-[18px] text-blue-800 self-start">
                До 30 апреля
              </p>
            </div>
          </SwiperSlide>
        </Swiper>

        <Swiper
          :slides-per-view="1"
          :loop="true"
          class="w-[408px] h-[320px]"
        >
          <SwiperSlide v-for="n in 3" :key="'second-' + n">
            <div class="w-full h-full bg-white rounded-[6px] flex items-center justify-center text-xl ">
              <div class="w-[336px] h-full flex justify-center">
                <div class="w-full h-full">
                  <p class="font-circe font-normal text-[24px] self-start mt-8 mb-10">
                    Товар дня
                  </p>
                  <img src="/smartphoneDay.svg"/>
                </div>
                <div class="w-full h-full mt-8">
                  <div class="flex flex-row gap-1">
                    <div class="w-[31px] h-[34px] rounded-[6px] bg-[rgba(237,237,237,1)] flex items-center justify-center">
                      <p class="text-[14px] text-bold">22</p>
                    </div>:
                    <div class="w-[31px] h-[34px] rounded-[6px] bg-[rgba(237,237,237,1)] flex items-center justify-center">
                      <p class="text-[14px] text-bold">57</p>
                    </div>:
                    <div class="w-[31px] h-[34px] rounded-[6px] bg-[rgba(237,237,237,1)] flex items-center justify-center">
                      <p class="text-[14px] text-bold">42</p>
                    </div>
                  </div>
                  <p class="font-circe font-normal text-[16px] mt-10 mb-2">
                    Смартфон Samsung Galaxy S23 256GB Phantom Black
                  </p>
                  <div class="flex flex-row gap-1 ">
                    <img src="/star.svg" class="h-[13px] mt-[3px]"/>
                    <img src="/star.svg" class="h-[13px] mt-[3px]"/>
                    <img src="/star.svg" class="h-[13px] mt-[3px]"/>
                    <img src="/star.svg" class="h-[13px] mt-[3px]"/>
                    <img src="/star.svg" class="h-[13px] mt-[3px]"/>
                    <p class="font-circe text-[14px] text-[#595959] mb-2">17 отзывов</p>
                  </div>
                  <p class="font-circe font-normal text-[16px] text-[#7D7D7D] leading-[18px] line-through mb-2 self-start">
                    529 990
                  </p>
                  <p class="font-circe text-[30px] font-normal text-[#333333] mb-2 self-start">
                   499 990 ₸
                   </p>
                </div>
              </div>
            </div>
          </SwiperSlide>
        </Swiper>
    </div>

      <!-- Кнопки под слайдерами -->
      <div class="flex justify-center gap-4 mt-4">
        <button class="w-[290px] h-[76px] flex items-center gap-4 px-4 bg-white rounded-lg shadow">
          <img src="/public/profile.svg" alt="profile" />
          <p class="text-[16px] leading-[18px] font-[400] tracking-[0px]" style="font-family: 'Circe', sans-serif;">
            Авторизуйтесь, чтобы применить бонусные тенге
          </p>
        </button>

        <button class="w-[290px] h-[76px] bg-white rounded-lg shadow flex items-center justify-center px-4">
          <img src="/public/shield.svg" alt="shield" />
          <p class="text-[16px] leading-[18px] font-[400] tracking-[0px]" style="font-family: 'Circe', sans-serif;">
            Страхование техники от утраты и повреждений
          </p>
        </button>

        <button class="w-[290px] h-[76px] bg-white rounded-lg shadow flex items-center justify-center px-4">
          <img src="/public/delivery.svg" alt="delivery" />
          <p class="text-[16px] leading-[18px] font-[400] tracking-[0px]" style="font-family: 'Circe', sans-serif;">
            Экспресс-доставка от 2 часов по Алматы 
          </p>
        </button>

        <button class="w-[290px] h-[76px] bg-white rounded-lg shadow flex items-center justify-center px-4">
          <img src="/public/card.svg" alt="card" />
          <p class="text-[16px] leading-[18px] font-[400] tracking-[0px]" style="font-family: 'Circe', sans-serif;">
            Оформляй в рассрочку и кредит не выходя из дома
          </p>
        </button>

        <button class="w-[290px] h-[76px] bg-white rounded-lg shadow flex items-center justify-center px-4">
          <img src="/public/trade.svg" alt="trade" />
          <p class="text-[16px] leading-[18px] font-[400] tracking-[0px]" style="font-family: 'Circe', sans-serif;">
            Обменяйте свой гаджет по программе Trade-in
          </p>
        </button>
      </div>
    </section>
  </div>

  <!-- Хиты продаж -->
  <div class="w-[1705px] h-[616px] mx-auto m">
    <div class="w-[460px] mb-5">
      <p class="font-circe font-normal text-[30px]">Хиты продаж</p>
      <div class="flex flex-row">
      <div class="border border-[#0E6CDD] w-[121px] h-[24px] rounded-[6px] border-[1px] mt-5 mr-3">
        <p class="font-circe font-normal text-[14px] text-center">
          Все категории
        </p>
      </div>

      <div class="border border-[#0E6CDD] w-[121px] h-[24px] rounded-[6px] border-[1px] mt-5 mr-3">
        <p class="font-circe font-normal text-[14px] text-center">
          Смартфоны
        </p>
      </div>

      <div class="border border-[#0E6CDD] w-[121px] h-[24px] rounded-[6px] border-[1px] mt-5 mr-3">
        <p class="font-circe font-normal text-[14px] text-center">
          Ноутбуки
        </p>
      </div>

      <div class="border border-[#0E6CDD] w-[121px] h-[24px] rounded-[6px] border-[1px] mt-5 mr-3">
        <p class="font-circe font-normal text-[14px] text-center">
          Умные часы
        </p>
      </div>
      </div>
    </div>
<div class="flex flex-row gap-6">
  <HitsSales />
  <HitsSales />
  <HitsSales />
  <HitsSales />
  <HitsSales />
  <HitsSales />
</div>
</div>
  <!-- Популярные категории -->
<div class="w-[1750px] h-[320px] mx-auto my-auto mt-12 mb-10">
  <p class="font-circe font-normal text-[30px]">
    Популярные категории
  </p>
  <div class="flex flex-row gap-6 mt-10">
    <PopularCategories />
    <PopularCategories />
    <PopularCategories />
    <PopularCategories />
    <PopularCategories />
    <PopularCategories />
    <PopularCategories />
    <PopularCategories />
  </div>
</div>

<div class="flex flex-row gap-6 mt-[90px] flex justify-center">
  <img src="/baners/Baner+Text.svg" loading="lazy" class="flex content-center"/>
  <img src="/baners/Baner+Text-1.svg" loading="lazy"/>
  <img src="/baners/Baner+Text-2.svg" loading="lazy"/>
</div>

<!-- Попоулярные бренды -->
<div class="flex flex-col justify-center w-[1705px] mx-auto mb-10 gap-6 mt-[90px]">
  <p class="font-circe font-normal text-[30px]">Популярные бренды</p>
<div class="flex flex-row gap-6 mt-10"> 
  <div class="flex justify-center self-center pt-[40px] w-[192px] h-[124px] bg-[rgba(14,108,221,0.05)]">
    <div class="h-[44px] w-[112px] flex items-center">
      <img src="/public/logo/dyson.svg" class="h-[42px]"/>
    </div>
  </div>

  <div class="flex justify-center self-center pt-[40px] w-[192px] h-[124px] bg-[rgba(14,108,221,0.05)]">
    <div class="h-[44px] w-[112px] flex items-center ">
      <img src="/public/logo/samsung.svg" class="h-[16px]"/>
    </div>
  </div>

  <div class="flex justify-center self-center pt-[40px] w-[192px] h-[124px] bg-[rgba(14,108,221,0.05)]">
    <div class="h-[44px] w-[112px] pl-[36px] flex items-center">
      <img src="/public/logo/apple.svg" class="h-[44px]"/>
    </div>
  </div>

  <div class="flex justify-center self-center pt-[40px] w-[192px] h-[124px] bg-[rgba(14,108,221,0.05)]">
    <div class="h-[44px] w-[112px] flex items-center ">
      <img src="/public/logo/robot.svg" class="h-[26px]"/>
    </div>
  </div>

  <div class="flex justify-center self-center pt-[40px] w-[192px] h-[124px] bg-[rgba(14,108,221,0.05)]">
    <div class="h-[44px] w-[112px] flex items-center">
      <img src="/public/logo/sony.svg" class="h-[20px]"/>
    </div>
  </div>

  <div class="flex justify-center self-center pt-[40px] w-[192px] h-[124px] bg-[rgba(14,108,221,0.05)]">
    <div class="h-[44px] w-[112px] flex items-center">
      <img src="/public/logo/logitech.svg" class="h-[34px]"/>
    </div>
  </div>

  <div class="flex justify-center self-center pt-[40px] w-[192px] h-[124px] bg-[rgba(14,108,221,0.05)]">
    <div class="h-[44px] w-[112px] flex items-center">
      <img src="/public/logo/tefal.svg" class="h-[22px]"/>
    </div>
  </div>

  <div class="flex justify-center self-center pt-[40px] w-[192px] h-[124px] bg-[rgba(14,108,221,0.05)]">
    <div class="h-[44px] w-[112px] flex items-center">
      <img src="/public/logo/asus.svg" class="h-[24px]"/>
    </div>
  </div>
</div> 
</div>


  <!-- Хиты продаж -->
  <div class="w-[1705px] h-[616px] mx-auto">
    <div class="w-[460px] mb-5">
      <p class="font-circe font-normal text-[30px]">Распродажа</p>
      <div class="flex flex-row">
      <div class="border border-[#0E6CDD] w-[121px] h-[24px] rounded-[6px] border-[1px] mt-5 mr-3">
        <p class="font-circe font-normal text-[14px] text-center">
          Все категории
        </p>
      </div>

      <div class="border border-[#0E6CDD] w-[121px] h-[24px] rounded-[6px] border-[1px] mt-5 mr-3">
        <p class="font-circe font-normal text-[14px] text-center">
          Смартфоны
        </p>
      </div>

      <div class="border border-[#0E6CDD] w-[121px] h-[24px] rounded-[6px] border-[1px] mt-5 mr-3">
        <p class="font-circe font-normal text-[14px] text-center">
          Ноутбуки
        </p>
      </div>

      <div class="border border-[#0E6CDD] w-[121px] h-[24px] rounded-[6px] border-[1px] mt-5 mr-3">
        <p class="font-circe font-normal text-[14px] text-center">
          Умные часы
        </p>
      </div>
      </div>
    </div>
<div class="flex flex-row gap-6">
  <HitsSales />
  <HitsSales />
  <HitsSales />
  <HitsSales />
  <HitsSales />
  <HitsSales />
</div>
</div>

<div class="mx-auto w-[1705px] relative mt-12 mb-12">
  <img src="/baners/baner.svg" loading="lazy"/>
  <div class="absolute inset-0 pt-15 mr-[900px]">
    <p class="font-circe font-normal text-[30px] place-self-center">Скидки до 50% на втрой товар встраиваемой техники.</p>
  </div>
</div>

<!-- Акции -->
<div class="w-[1705px] mx-auto">
  <div class="flex flex-row items-center gap-4">
    <p class="font-circe font-normal text-[30px]">Акции</p>
    <div class="w-[28px] h-[28px] bg-[rgba(14,108,221,0.05)] rounded-[6px] flex items-center grid place-content-center">
      <img src="/rightArrow.svg"/>
    </div>
  </div>

  <div class="flex flex-row gap-6 mt-10">
    <div class="flex flex-col">
      <img src="/baners/promoBaner1.svg" loading="lazy"/>
      <p class="font-circe font-normal text-[18px] ml-2 mt-5">
        Черная пятница в разгаре, скидки до 80%! 
      </p>
    </div>
    <div class="flex flex-col">
      <img src="/baners/promoBaner2.svg" loading="lazy"/>
      <p class="font-circe font-normal text-[18px] ml-2 mt-5">
        Рассрочка 0-0-24 на всю технику Apple.   
      </p>
    </div>
    <div class="flex flex-col">
      <img src="/baners/promoBaner3.svg" loading="lazy"/>
      <p class="font-circe font-normal text-[18px] ml-2 mt-5">
        Скидки на умные часы в самом разгаре!  
      </p>
    </div>
    <div class="flex flex-col">
      <img src="/baners/promoBaner4.svg" loading="lazy"/>
      <p class="font-circe font-normal text-[18px] ml-2 mt-5">
        Весь декабрь, объявляется месяцем игровых <br> мониторов.   
      </p>
    </div>
  </div>
</div>

<!-- Рекомендуем -->
<div class="w-[1705px] h-[616px] mx-auto">
    <div class="w-[460px] mb-5">
      <p class="font-circe font-normal text-[30px]">Рекомендуем</p>
      <div class="flex flex-row">
      <div class="border border-[#0E6CDD] w-[121px] h-[24px] rounded-[6px] border-[1px] mt-5 mr-3">
        <p class="font-circe font-normal text-[14px] text-center">
          Все категории
        </p>
      </div>

      <div class="border border-[#0E6CDD] w-[121px] h-[24px] rounded-[6px] border-[1px] mt-5 mr-3">
        <p class="font-circe font-normal text-[14px] text-center">
          Смартфоны
        </p>
      </div>

      <div class="border border-[#0E6CDD] w-[121px] h-[24px] rounded-[6px] border-[1px] mt-5 mr-3">
        <p class="font-circe font-normal text-[14px] text-center">
          Ноутбуки
        </p>
      </div>

      <div class="border border-[#0E6CDD] w-[121px] h-[24px] rounded-[6px] border-[1px] mt-5 mr-3">
        <p class="font-circe font-normal text-[14px] text-center">
          Умные часы
        </p>
      </div>
      </div>
    </div>
<div class="flex flex-row gap-6">
  <HitsSales />
  <HitsSales />
  <HitsSales />
  <HitsSales />
  <HitsSales />
  <HitsSales />
</div>
</div>


<!-- Блог -->
<div class="w-[1705px] mx-auto mt-5">
  <div class="flex flex-row items-center gap-4">
    <p class="font-circe font-normal text-[30px]">Блог</p>
    <div class="w-[28px] h-[28px] bg-[rgba(14,108,221,0.05)] rounded-[6px] flex items-center grid place-content-center">
      <img src="/rightArrow.svg"/>
    </div>
  </div>
  <div class="flex flex-row gap-6">
    <div class="flex flex-col">
      <div class="w-[264px] h-[192px] bg-[rgba(14,108,221,0.05)] mb-9"></div>
      <p class="font-circe font-normal text-[18px] mb-4">
        PlayStation 5 Slim: новая <br> ревизия, которая понравится <br> вам больше обычной
      </p>
      <p class="font-circe font-normal text-[14px] text-[rgba(125,125,125,1)]">
        Обзор / 28 июня 2022
      </p>
    </div>

    <div class="flex flex-col">
      <div class="w-[264px] h-[192px] bg-[rgba(14,108,221,0.05)] mb-9"></div>
      <p class="font-circe font-normal text-[18px] mb-4">
        Показан дизайн OnePlus 12R
      </p>
      <p class="font-circe font-normal text-[14px] text-[rgba(125,125,125,1)]">
        Обзор / 28 июня 2022
      </p>
    </div>

    <div class="flex flex-col">
      <div class="w-[264px] h-[192px] bg-[rgba(14,108,221,0.05)] mb-9"></div>
      <p class="font-circe font-normal text-[18px] mb-4">
        Обзор «Яндекс Станции Миди»:<br> компромисс без компромиссов
      </p>
      <p class="font-circe font-normal text-[14px] text-[rgba(125,125,125,1)]">
        Обзор / 28 июня 2022
      </p>
    </div>

    <div class="flex flex-col">
      <div class="w-[264px] h-[192px] bg-[rgba(14,108,221,0.05)] mb-9"></div>
      <p class="font-circe font-normal text-[18px] mb-4">
        PlayStation 5 Slim: новая <br> ревизия, которая понравится <br> вам больше обычной
      </p>
      <p class="font-circe font-normal text-[14px] text-[rgba(125,125,125,1)]">
        Обзор / 28 июня 2022
      </p>
    </div>

    <div class="flex flex-col">
      <div class="w-[264px] h-[192px] bg-[rgba(14,108,221,0.05)] mb-9"></div>
      <p class="font-circe font-normal text-[18px] mb-4">
        PlayStation 5 Slim: новая <br> ревизия, которая понравится <br> вам больше обычной
      </p>
      <p class="font-circe font-normal text-[14px] text-[rgba(125,125,125,1)]">
        Обзор / 28 июня 2022
      </p>
    </div>

    <div class="flex flex-col">
      <div class="w-[264px] h-[192px] bg-[rgba(14,108,221,0.05)] mb-9"></div>
      <p class="font-circe font-normal text-[18px] mb-4">
        PlayStation 5 Slim: новая <br> ревизия, которая понравится <br> вам больше обычной
      </p>
      <p class="font-circe font-normal text-[14px] text-[rgba(125,125,125,1)]">
        Обзор / 28 июня 2022
      </p>
    </div>
  </div>
</div>



<div class="w-[1650px] h-[484px] flex justify-between items-center mx-auto mt-10 border border-[rgba(14,108,221,0.2)]">
  <div class="ml-10">
    <p class="font-circe font-normal text-[30px]">
      Интернет-магазин в Алматы
    </p>
    <p class="font-circe font-normal text-[16px] text-[rgba(51,51,51,1)]">
      itl.b2c — магазин умной техники и электроники для вашего дома.<br><br>
    Здесь вы найдете товары под свои предпочтения: от видеотехники и роботов пылесовов. Работаем с <br>
    проверенными производителями с 2005 года. Доставляем товары точно в срок.<br> <br>
    Покупка товара проста только на первый взгляд. Нужно думать о том, как оформить доставку, кто соберет <br>
    шкаф или установит кондиционер. В нашем магазине эти услуги уже продуманы. <br> <br>
    Думайте только о подборе товаров в каталоге. Для этого предлагаем комплексный подход — наша команда <br>
    выполнит все задачи!<br> <br>
    </p>
    <button class="flex items-center justify-center gap-2 w-[112px] h-[48px] px-5 py-3 rounded-md bg-[#FFD740] ml-0 md:ml-4">
      <span class="font-circe font-normal text-[16px] text-center whitespace-nowrap">Подробнее</span>
    </button>
  </div>

  <div>
    <div v-if="loading" class="w-[778px] h-[370px] bg-blue-50 animate-pulse"></div>
    <div v-else>
      <img src="/Photo.svg" class="w-[778px] h-[370px]" loading="lazy"/>
    </div>
  </div>
</div>


<div class="w-[1750px] mx-auto mt-15 mb-15">
  <p class="font-circe font-normal text-[30px] ml-12 mb-10">Вы смотрели</p>
  <div class="border w-[192px] h-[310px] border-[rgba(14,108,221,0.2)] rounded-[6px] ml-12">
    <img src="/public/iphone.svg" class="mx-auto mb-4 h-[120px] mt-8" />
    <div class="ml-[25px]">
      <p class="font-circe text-[16px] font-normal text-[#333333] mb-2 self-start">
        Смартфон Apple <br> iPhone  14 Pro Max
      </p>
      <p class="font-circe font-normal text-[14px] text-[#7D7D7D] leading-[18px] line-through mb-2 self-start">
        529 990
      </p>
      <p class="font-circe text-[24px] font-normal text-[#333333] mb-2 self-start">
        499 990 ₸
      </p>
    </div>
  </div>
</div>
</template>

<script setup>
import { Swiper, SwiperSlide } from 'swiper/vue'
import 'swiper/css'

const loading = ref(true)
onMounted(() => {
  loading.value = false
})
</script>