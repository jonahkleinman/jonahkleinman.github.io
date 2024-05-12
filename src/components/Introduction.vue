<template>
  <div class="bg-gray-100 py-12">
    <div class="max-w-6xl mx-auto px-4">
      <div class="text-center mb-8">
        <h1 class="text-6xl font-bold text-gray-900">Hi, I'm Jonah</h1>
        <p class="text-gray-600 mt-2 text-xl">And I'm a <span class="typing"></span></p>
      </div>
    </div>
  </div>
</template>

<script>
import Typed from 'typed.js';
document.addEventListener('DOMContentLoaded', function() {
  var typed = new Typed(".typing", {
    strings: ["Freelance Developer", "UX Designer", "Software Engineer", "Full-stack Developer", "Programmer"],
    typeSpeed: 100,
    backSpeed: 60,
    loop: true
  });
});
</script>
