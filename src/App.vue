<style>
/* Tailwind css import */
@import "@/assets/index.css";
</style>

<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import { AcademicCapIcon, ChipIcon, HomeIcon } from "@heroicons/vue/outline";
</script>

<template>
  <div class="">
    <header class="bg-white shadow">
      <div class="max-w-7xl mx-auto py-6 px-4 sm:px-6 lg:px-8">
        <h1 class="text-3xl font-bold text-gray-900">Header</h1>
      </div>
    </header>
    <main>
      <div class="mx-auto py-6">
        <!-- Replace with your content -->
        <div class="px-4 py-6 sm:px-0">
          <RouterView />
        </div>
        <!-- /End replace -->
      </div>
      <section
        id="bottom-navigation"
        class="block fixed inset-x-0 bottom-0 z-10 bg-slate-100"
      >
        <div id="tabs" class="flex justify-between">
          <RouterLink
            to="/"
            class="w-full focus:text-teal-500 hover:text-teal-500 justify-center inline-block text-center pt-2 pb-2"
          >
            <HomeIcon class="h-8 w-8 inline-block mb-2" />
            <span class="block text-xs">Home</span>
          </RouterLink>
          <RouterLink
            to="/about"
            class="w-full focus:text-teal-500 hover:text-teal-500 justify-center inline-block text-center pt-2 pb-2"
          >
            <ChipIcon class="h-8 w-8 inline-block mb-2" />
            <span class="block text-xs">Home</span>
          </RouterLink>
          <RouterLink
            to="/other"
            class="w-full focus:text-teal-500 hover:text-teal-500 justify-center inline-block text-center pt-2 pb-2"
          >
            <AcademicCapIcon class="h-8 w-8 inline-block mb-2" />
            <span class="block text-xs">Home</span>
          </RouterLink>
        </div>
      </section>
    </main>
  </div>
</template>
