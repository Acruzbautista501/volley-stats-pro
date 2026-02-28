<script setup lang="ts">
import AppHeader from './AppHeader.vue'
import AppSidebar from './AppSidebar.vue'
</script>

<template>
  <div class="flex h-screen bg-gray-100">

    <!-- Sidebar -->
    <AppSidebar />

    <!-- Contenido -->
    <div class="flex flex-col flex-1">

      <!-- Header -->
      <AppHeader />

      <!-- Vista dinámica -->
      <main class="p-6 overflow-y-auto">
        <RouterView />
      </main>

    </div>
  </div>
</template>