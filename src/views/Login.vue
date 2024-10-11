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
  <div class="login">
    <h2>Login</h2>
    <form @submit.prevent="login">
      <div>
        <label for="username">Usuario:</label>
        <input id="username" v-model="username" type="text" required>
      </div>
      <div>
        <label for="password">Contraseña:</label>
        <input id="password" v-model="password" type="password" required>
      </div>
      <button type="submit">Iniciar sesión</button>
    </form>
  </div>
</template>

<style scoped>
.login {
  max-width: 300px;
  margin: 0 auto;
}
form {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}
</style>