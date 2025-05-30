<template>
    <div class="flex flex-row gap-7">
  <div class="w-[264px] h-[496px] rounded-[6px] border border-[rgba(14,108,221,0.2)] overflow-hidden relative p-4 flex flex-col justify-between">

  <div class="absolute top-4 left-4 space-y-1 z-10">
    <div class="w-[108px] h-[24px] bg-[#34A853] rounded-[6px] flex items-center justify-center">
      <p class="font-circe text-[14px] text-white">Товар недели</p>
    </div>
    <div class="w-[93px] h-[24px] bg-[#E31E24] rounded-[6px] flex items-center justify-center">
      <p class="font-circe text-[14px] text-white">Скидка 6%</p>
    </div>
  </div>

  <!-- Контент карточки -->
  <div class="flex flex-col items-center text-left flex-1 mt-10">
    <img src="/public/iphone.svg" class="mx-auto mb-4" />

    <div class="flex items-center gap-2 mb-2 self-start">
      <img src="/star.svg" class="w-4 h-4" />
      <p class="font-circe text-[14px] text-[#595959]">4.8</p>
    </div>

    <p class="font-circe text-[16px] font-normal text-[#333333] mb-2 self-start">
      Смартфон Apple iPhone 14 Pro Max
    </p>

    <p class="font-circe font-normal text-[14px] leading-[24px] mb-2 self-start">
      В наличии в
      <a href="#" class="text-[#0E6CDD] hover:underline">5 магазинах</a>
    </p>

    <p class="font-circe font-normal text-[14px] text-[#7D7D7D] leading-[18px] line-through mb-2 self-start">
      529 990
    </p>

    <p class="font-circe text-[18px] font-normal text-[#333333] mb-2 self-start">
      499 990 ₸
    </p>

  <div class="self-start flex items-baseline gap-4">
    <button class="bg-[#FFD740] text-[#333333] text-[14px] font-circe py-2 px-4 rounded-[6px] w-[125px] h-[44px] flex items-center justify-center gap-1 shrink-0">
      <img src="/plus.svg" class="relative top-[2px] w-4 h-4" />
        В корзину
    </button>

    <div class="flex gap-3 items-center">
      <img src="/heartLight.svg" alt="heart" class="w-6 h-6" />
      <img src="/icon.svg" alt="icon" class="w-6 h-6" />
    </div>
  </div>



  </div>
  </div>

  
  
</div>
</template>