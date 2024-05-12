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
  </div>
</template>

<script>
export default {
  data() {
    return {
      jobs: [
        {
          id: 1,
          title: "Development Team - The Pilot Club",
          period: "May 2023 - Present",
          duties: [
            "Led the design and development of cutting-edge features for The Pilot Club's Discord bot, enhancing functionality and boosting user engagement dramatically.",
            "Coordinated cross-functional teams to optimize project delivery, maintaining rigorous quality and efficiency standards."
          ]
        },
        {
          id: 2,
          title: "Lead Developer - School House Points System",
          period: "January 2023 - Present",
          duties: [
            "Architected and developed a house point system for a lower school using Firebase, Vue, and Tailwind CSS, fostering a gamified and interactive environment for students.",
            "Ensured scalable and secure backend solutions with Firebase to manage real-time data efficiently."
          ]
        },
        {
          id: 3,
          title: "Software Engineer - VX",
          period: "April 2023 - Present",
          duties: [
            "Developed and deployed a network authentication bot, enhancing system security and streamlining user verification processes."
          ]
        },
        {
          id: 4,
          title: "Web Developer - ZAB Web Team",
          period: "April 2023 - May 2023",
          duties: [
            "Contributed to the enhancement of the website's UI/UX, leading to a more intuitive and user-friendly experience.",
            "Addressed and resolved various front-end bugs, enhancing site performance and stability."
          ]
        },
        {
          id: 5,
          title: "Co-Developer - FlightBot",
          period: "January 2023 - Present",
          duties: [
            "Played a key role in the continuous development of the FlightBot, expanding its reach across over 50 new servers.",
            "Participated in redesigning the Flight Crew Portal with Laravel, modernizing the previous system and improving operational efficiency."
          ]
        }
      ]
    };
  }
}
</script>
