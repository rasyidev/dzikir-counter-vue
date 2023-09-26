<template>
  <div class="h-screen w-screen justify-center flex">
    <div class="px-2 lg:px-0 w-11/12 xs:w-9/12 lg:w-8/12 h-4/6 m-auto p-5 bg-gray-200 rounded-md flex items-center justify-center relative">
      <button class="px-4 py-1 bg-teal-500 h-auto hover:bg-teal-600 active:bg-teal-700 rounded-lg text-gray-50 absolute max-[500px]:bottom-6 max-[500px]:left-2 min-[501px]:right-2 min-[501px]:top-2 text-xl" @click="jumlahSet=0">Reset</button>
      <div class="align-middle items-end">
        <h1 class="text-5xl text-center">Dzikir Counter</h1>
        <p class="text-9xl text-center my-4">{{ jumlahSet }}</p>
        <div class="text-cente flex justify-center">
          <PlusIcon class="text-teal-500 w-10 h-auto hover:text-teal-600 active:text-teal-700 block select-none" @click="jumlahSet++"/>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

import PlusIcon from './components/icons/PlusIcon.vue'

const jumlahSet = ref(0);

</script>