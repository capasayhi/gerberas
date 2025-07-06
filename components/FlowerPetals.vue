<template>
  <div>
     <div class="flower-container">
      <!-- petals-outer -->
      <div class="flex justify-center items-center top-0 right-0 left-0 bottom-0 absolute max-w-[100%] max-h-[100%] ">
        <!-- petal -->
        <div
        v-for="i in 24"
          :key="i"
          class=" absolute h-20  w-[600px] bg-fuchsia-800 max-h-[100%] rounded-l-[50%] rounded-r-[50%] border-white"
          :style="{ transform: `rotate(${i * 20}deg)` }"
        />
      </div>
      <!-- petals-inner -->
      <div class=" m-auto flex justify-center items-center top-0 right-0 left-0 bottom-0 absolute max-w-[500px] max-h-[100%] rotate-30">
        <!-- petal -->
        <div v-for="i in 12" :key="i" class="petal rounded-l-[50%] rounded-r-[50%] absolute h-20  bg-fuchsia-400 w-[500px]" :style="{ transform: `rotate(${i * 30}deg)` }"/>
      </div>
      <!-- flower-center -->
      <div class="m-auto rounded-full top-0 right-0 left-0 bottom-0 absolute w-[150px] h-[150px] bg-yellow-300"/>
    </div>
  </div>
</template>

<script lang="ts" setup>

</script>

<style>

</style>