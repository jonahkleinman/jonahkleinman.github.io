<template>
  <div>
    <h2 class="text-4xl font-bold text-center text-gray-900 mb-8">Professional Experience</h2>
    <div class="space-y-8">
      <div v-for="job in jobs" :key="job.id" class="bg-white shadow-lg rounded-lg p-8 hover:bg-gray-50 transition duration-300 ease-in-out">
        <h3 class="text-2xl font-bold text-gray-800">{{ job.title }}</h3>
        <p class="text-gray-600 italic">{{ job.period }}</p>
        <ul class="list-disc pl-5 mt-4 text-gray-700">
          <li v-for="duty in job.duties" :key="duty">{{ duty }}</li>
        </ul>
      </div>
    </div>
    <h2 class="text-4xl font-bold text-center text-gray-900 mb-8 mt-12">Personal Projects</h2>
    <div class="space-y-8">
      <div v-for="project in personalProjects" :key="project.id" class="bg-white shadow-lg rounded-lg p-8 hover:bg-gray-50 transition duration-300 ease-in-out">
        <h3 class="text-2xl font-bold text-gray-800">{{ project.title }}</h3>
        <ul class="list-disc pl-5 mt-4 text-gray-700">
          <li v-for="duty in project.duties" :key="duty">{{ duty }}</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      jobs: [
        {
          id: 3,
          title: "Software Engineer - VX",
          period: "April 2024 - Present",
          duties: [
            "Developed an automation bot for the network sign-on process, enhancing system accessibility and user efficiency."
          ]
        },
        {
          id: 4,
          title: "Web Developer - ZAB Web Team",
          period: "April 2024 - May 2024",
          duties: [
            "Contributed to the enhancement of the website's UI/UX, leading to a more intuitive and user-friendly experience.",
            "Addressed and resolved various front-end bugs, enhancing site performance and stability."
          ]
        },
        {
          id: 6,
          title: "Development Team - The Pilot Club",
          period: "May 2023 - Present",
          duties: [
            "Spearheaded the development of The Pilot Club's Discord bot, implementing new features efficiently under direction from the Development Team Lead.",
            "Managed tech debt and coordinated with a cross-functional team to ensure efficient communication and timely project delivery.",
            "Participated in developing the Flight Crew Portal using Laravel, overhauling the previous outdated system."
          ]
        },
        {
          id: 7,
          title: "Co-Developer - FlightBot",
          period: "January 2023 - Present",
          duties: [
            "Played a key role in the continuous development of the bot, expanding its reach across over 50 new servers.",
          ]
        },
      ],
      personalProjects: [
        {
          id: 1,
          title: "Professional Portfolio",
          duties: [
            "Designed this dynamic Vue.js application to showcase professional experiences and projects.",
            "Utilized Tailwind CSS for styling to ensure the application is visually appealing and responsive across different devices.",
            "Integrated advanced Vue.js features such as components for reusable UI elements."
          ]
        },
        {
          id: 2,
          title: "Lead Developer - School House Points System",
          duties: [
            "Architected and developed a house point system for a lower school using Firebase, Vue, and Tailwind CSS, fostering a gamified and interactive environment for students.",
            "Ensured scalable and secure backend solutions with Firebase to manage real-time data efficiently."
          ]
        },
        {
          id: 5,
          title: "Lead Developer - School Assignment System",
          duties: [
            "Conceptualized, designed, and implemented an alternative assignment tracking system utilized by over 200 students and faculty daily.",
          ]
        },
      ]
    };
  }
}
</script>
