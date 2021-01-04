<template>
  <header class="flex justify-between py-5 items-center mb-5">
    <h1 class="text-md text-gray-500 uppercase">{{ title }}</h1>

    <button class="hover:bg-blue-200 hover:text-blue-800 group flex items-center rounded-md bg-blue-100 text-blue-600 text-sm font-medium px-4 py-2 focus:outline-none focus:ring-2 focus:ring-blue-400 focus:ring-opacity-75 transition-colors">
      <svg class="group-hover:text-blue-600 text-blue-500 mr-2" width="12" height="20" fill="currentColor">
        <path fill-rule="evenodd" clip-rule="evenodd" d="M6 5a1 1 0 011 1v3h3a1 1 0 110 2H7v3a1 1 0 11-2 0v-3H2a1 1 0 110-2h3V6a1 1 0 011-1z"/>
      </svg>
      Add
    </button>
  </header>
</template>

<script>
export default {
  props: ['title']
}
</script>