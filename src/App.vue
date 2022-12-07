<template>
  <div class="w-full h-full flex justify-center items-center">
    <div>
      <div class="w-full max-w-2xl p-4 rounded bg-red-400 text-white">
        <div class="border-2 rounded flex flex-col md:flex-row md:items-center md:gap-8 p-4">
          <img src="/assets/santa.svg" alt="" class="max-w-[12em]" />
          <div>
            <h1 class="font-serif text-4xl">Happy Holidays!</h1>
            <div class="mt-4 bg-white text-black p-2 rounded">TO: {{ to }}</div>
            <div class="mt-2 bg-white text-black p-2 rounded">FROM: {{ from }}</div>
          </div>
        </div>
      </div>
      <form class="flex flex-col gap-2 mt-5">
        <label for="to" class="w-full -mb-2">To: </label>
        <input
          v-model="to"
          type="text"
          id="to"
          class="bg-gray-50 border p-2 rounded-lg text-sm focus:outline-gray-300"
        />
        <label for="from" class="w-full -mb-2">From: </label>
        <input
          v-model="from"
          type="text"
          id="from"
          class="bg-gray-50 border p-2 rounded-lg text-sm focus:outline-gray-300"
        />
      </form>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const to = ref('')
const from = ref('')
</script>
