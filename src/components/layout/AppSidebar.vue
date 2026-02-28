<script setup lang="ts">
import { useLayout } from '@/composables/useLayout'

const { sidebarOpen } = useLayout()
</script>

<template>
  <aside
    class="bg-gray-900 text-white h-screen transition-all duration-300"
    :class="sidebarOpen ? 'w-64' : 'w-0 overflow-hidden'"
  >
    <div v-if="sidebarOpen" class="p-4 space-y-4">

      <h2 class="text-xl font-bold">Liga Fútbol</h2>

      <nav class="space-y-2">
        <RouterLink to="/dashboard" class="block hover:bg-gray-700 p-2 rounded">
          Dashboard
        </RouterLink>

        <RouterLink to="/teams" class="block hover:bg-gray-700 p-2 rounded">
          Equipos
        </RouterLink>

        <RouterLink to="/matches" class="block hover:bg-gray-700 p-2 rounded">
          Partidos
        </RouterLink>

        <RouterLink to="/stats" class="block hover:bg-gray-700 p-2 rounded">
          Estadísticas
        </RouterLink>
      </nav>

    </div>
  </aside>
</template>