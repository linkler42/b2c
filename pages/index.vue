<template>
  <div class="w-full max-w-[1920px] bg-[#F1F6FD] mb-[25px] px-4 lg:px-8 mx-auto">
    <section class="flex flex-col py-10 px-4 lg:px-8">
      
      <!-- Слайдеры -->
      <div class="flex gap-6 justify-center max-w-[1680px] mx-auto mb-6">
        <Swiper
          :slides-per-view="1"
          :loop="true"
          class="w-[1200px] h-[320px]"
        >
          <SwiperSlide v-for="n in 3" :key="'first-' + n">
            <div class="w-full h-full flex items-center justify-center text-2xl font-bold bg-gray-200 rounded-xl">
              Slide {{ n }}
            </div>
          </SwiperSlide>
        </Swiper>

        <Swiper
          :slides-per-view="1"
          :loop="true"
          class="w-[408px] h-[320px]"
        >
          <SwiperSlide v-for="n in 3" :key="'second-' + n">
            <div class="w-full h-full bg-white rounded-[6px] flex items-center justify-center text-xl font-semibold">
              Slide {{ n }}
            </div>
          </SwiperSlide>
        </Swiper>
      </div>

      <!-- Кнопки под слайдерами -->
      <div class="flex justify-center gap-4 mt-4">
        <button class="w-[290px] h-[76px] flex items-center gap-4 px-4 bg-white rounded-lg shadow">
          <img src="/profile.svg" alt="profile" />
          <p class="text-[16px] leading-[18px] font-[400] tracking-[0px]" style="font-family: 'Circe', sans-serif;">
            Авторизуйтесь, чтобы применить бонусные тенге
          </p>
        </button>

        <button class="w-[290px] h-[76px] bg-white rounded-lg shadow flex items-center justify-center px-4">
          <img src="/shield.svg" alt="shield" />
          <p class="text-[16px] leading-[18px] font-[400] tracking-[0px]" style="font-family: 'Circe', sans-serif;">
            Страхование техники от утраты и повреждений
          </p>
        </button>

        <button class="w-[290px] h-[76px] bg-white rounded-lg shadow flex items-center justify-center px-4">
          <img src="/delivery.svg" alt="delivery" />
          <p class="text-[16px] leading-[18px] font-[400] tracking-[0px]" style="font-family: 'Circe', sans-serif;">
            Экспресс-доставка от 2 часов по Алматы 
          </p>
        </button>

        <button class="w-[290px] h-[76px] bg-white rounded-lg shadow flex items-center justify-center px-4">
          <img src="/card.svg" alt="card" />
          <p class="text-[16px] leading-[18px] font-[400] tracking-[0px]" style="font-family: 'Circe', sans-serif;">
            Оформляй в рассрочку и кредит не выходя из дома
          </p>
        </button>

        <button class="w-[290px] h-[76px] bg-white rounded-lg shadow flex items-center justify-center px-4">
          <img src="/trade.svg" alt="trade" />
          <p class="text-[16px] leading-[18px] font-[400] tracking-[0px]" style="font-family: 'Circe', sans-serif;">
            Обменяйте свой гаджет по программе Trade-in
          </p>
        </button>
      </div>
    </section>
  </div>

  <div class="w-[1650px] h-[616px] mx-auto my-auto mt-5 mb-5">
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

  <!-- Товары в Хиты продаж -->
<div class="flex flex-row gap-6">
  <HitsSales />
  <HitsSales />
  <HitsSales />
  <HitsSales />
  <HitsSales />
  <HitsSales />
</div>


</div>
</template>

<script setup>
import { Swiper, SwiperSlide } from 'swiper/vue'
import 'swiper/css'
</script>