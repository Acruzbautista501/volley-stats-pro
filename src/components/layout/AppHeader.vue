<script setup lang="ts">
import { useLayout } from '@/composables/useLayout'

const { toggleSidebar } = useLayout()
</script>

<template>
  <header class="bg-white border-b shadow-sm">
    <div class="flex items-center justify-between px-4 py-3">

      <!-- Botón -->
      <button
        @click="toggleSidebar"
        class="p-2 rounded-lg hover:bg-gray-100 transition"
      >
        ☰
      </button>

      <h1 class="text-lg font-semibold">
        Liga Fútbol Admin
      </h1>

      <div class="text-sm text-gray-500">
        Panel Administrativo
      </div>

    </div>
  </header>
</template>