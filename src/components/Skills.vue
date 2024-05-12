<template>
  <div>
    <h2 class="text-4xl font-bold text-center text-gray-900 mb-8">Programming Skills</h2>
    <div class="grid grid-cols-2 gap-4">
      <div v-for="skill in skills" :key="skill.name" class="bg-white shadow-lg rounded-lg p-8 hover:bg-gray-50 transition duration-300 ease-in-out">
        <h3 class="text-2xl font-bold text-gray-800">{{ skill.name }}</h3>
        <p class="mt-4 text-gray-700">{{ skill.description }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      skills: [
        {
          name: "JavaScript",
          description: "Proficient in using JavaScript for both client-side and server-side scripting, enabling interactive web pages and API services."
        },
        {
          name: "Python",
          description: "Expert in Python, focusing on web development with frameworks like Django and Flask, and automation scripts."
        },
        {
          name: "PHP",
          description: "Skilled in PHP, adept at building dynamic and interactive websites using modern frameworks like Laravel."
        },
        {
          name: "TypeScript",
          description: "Advanced proficiency in TypeScript, enhancing JavaScript code reliability and maintainability through strict syntactical and type checks."
        },
        {
          name: "React",
          description: "Experienced with React, creating efficient and reusable UI components, managing state with hooks, and handling complex user interactions."
        },
        {
          name: "Vue",
          description: "Skilled in Vue.js, focusing on building interactive and performant single-page applications with a reactive and composable UI."
        }
      ]
    };
  }
}
</script>

