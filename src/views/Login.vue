<script setup lang="ts">
import { ref } from 'vue'

const username = ref('')
const password = ref('')

const login = () => {
  // Aquí iría la lógica de login
  console.log('Intento de login con:', username.value, password.value)
}
</script>

<template>
  <div class=" flex  justify-center items-center min-h-screen pb-[10%]">
    <div class="w-full max-w-[400px] bg-white  rounded-lg shadow-md p-4 text-black">
      <h2 class="text-2xl font-bold mb-6 text-center">Login</h2>
      <form @submit.prevent="login" class="space-y-4">
        <div>
          <label for="username" class="block mb-1">Usuario:</label>
          <input id="username" v-model="username" type="text" required class=" text-white w-full px-3 py-2 border rounded-md">
        </div>
        <div>
          <label for="password" class="block mb-1">Contraseña:</label>
          <input id="password" v-model="password" type="password" required class=" text-white w-full px-3 py-2 border rounded-md">
        </div>
        <router-link to="/" class="w-full block">
          <button type="button" class="w-full bg-blue-500 text-white py-2 rounded-md hover:bg-blue-600">Iniciar sesión</button>
        </router-link>
      </form>
    </div>
  </div>
</template>

<style scoped>
/* Puedes eliminar los estilos scoped ya que ahora usamos Tailwind */
</style>
