<template>
<div v-if="loading">
    <div class="bg-blue-50 w-[192px] h-[240px] rounded-[6px] my-auto mt-5 animate-pulse"></div>
</div>
<div v-else>
    <div class="w-[192px] h-[240px] my-auto mt-5">
          <div class="w-[192px] h-[192px] rounded-[6px] bg-[rgba(14,108,221,0.07)] grid place-items-center mb-5">
            <img src="/public/iphone.svg" class="h-[128px]"/>
        </div>
        <p class="font-circe font-normal text-[16px] text-center">
            Смартфоны
        </p>
    </div>
</div>
</template>

<script setup>
   const loading = ref(true)
   onMounted(() => {
  loading.value = false
})
</script>