<template>
  <article
    v-for="resource in storedResources"
    :key="resource.id"
    class="dark:hover:bg-gray-500 hover:shadow-lg bg-white dark:bg-gray-700 rounded-md overflow-hidden p-5 shadow-sm mb-4 transition-all"
  >
    <a :href="resource.link" class="">
      <header class="flex items-center justify-between">
        <h2
          class="font-semibold text-lg leading-tight text-gray-700 dark:text-gray-50"
        >
          {{ resource.title }}
        </h2>
        <button class="transition-colors text-gray-300 hover:text-red-600">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            width="24"
            height="24"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M10 14l2-2m0 0l2-2m-2 2l-2-2m2 2l2 2m7-2a9 9 0 11-18 0 9 9 0 0118 0z"
            />
          </svg>
        </button>
      </header>

      <p class="mt-2 text-gray-500 dark:text-gray-200">
        {{ resource.description }}
      </p>
    </a>
  </article>
</template>

<script>
export default {
  data() {
    return {
      storedResources: [
        {
          id: "official-guide",
          title: "Official Guide",
          description: "The official Vue.js documentation.",
          link: "https://vuejs.org",
        },
        {
          id: "google",
          title: "Google",
          description: "Learn go google...",
          link: "https://google.com",
        },
      ],
    };
  },
};
</script>