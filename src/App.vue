<template>
  <Header title="Remember Me" />
  <ResourceList />
  <button class="rounded-lg w-full">
    <a href="#" class="hover:text-gray-500 hover:bg-blue-50 hover:border-blue-200 transition-colors w-full flex items-center justify-center rounded-lg border-2 border-dashed border-blue-100 text-sm font-medium py-5 px-3 text-gray-400"
    >
      Add resource
    </a>
  </button>
</template>

<script>
import Header from './components/Header.vue'
import ResourceList from './components/ResourceList.vue'

export default {
  name: 'App',
  components: {
    Header,
    ResourceList
  }
}
</script>
