<script setup>
import Navbar from './components/Navbar.vue';
import Sidebar from './components/Sidebar.vue';
</script>

<template>
  <div>
    <Navbar />

    <div class="flex overflow-hidden bg-white pt-16">

      <Sidebar />

      <div class="bg-gray-900 opacity-50 hidden fixed inset-0 z-10" id="sidebarBackdrop"></div>
      <div id="main-content" class="h-full w-full bg-gray-50 relative overflow-y-auto lg:ml-64">
        <main>


          <RouterView />

        </main>
      </div>
    </div>
  </div>
</template>
