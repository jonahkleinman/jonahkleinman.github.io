<template>
  <div id="app" class="min-h-screen bg-gray-100 text-white">
    <div class="container mx-auto py-12">
      <introduction class="mb-8" />
      <experience class="mb-8" />
      <skills class="mb-8" />
      <hr>
      <icons />
    </div>
  </div>
</template>

<script setup>
import Experience from "@/components/Experience.vue";
import Skills from "@/components/Skills.vue";
import Icons from "@/components/Icons.vue";
import Introduction from "@/components/Introduction.vue";
</script>

<style>
@import 'tailwindcss/base';
@import 'tailwindcss/components';
@import 'tailwindcss/utilities';
</style>
