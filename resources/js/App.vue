<script setup>
import { ref } from 'vue';

const series = ref(0);
</script>

<template>
  <main class="templa">
    <h1>Templa</h1>
    <p class="eslogan">Tu cuerpo, bien afilao.</p>

    <section class="prueba">
      <p>Si ves esto, Vue funciona dentro de Laravel.</p>
      <button @click="series++">Hacer una serie</button>
      <p>Series hechas: <strong>{{ series }}</strong></p>
    </section>
  </main>
</template>

<style scoped>
.templa {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 1rem;
  background: #111;
  color: #f5f5f5;
  font-family: system-ui, sans-serif;
  text-align: center;
  padding: 1rem;
}

h1 {
  font-size: 3rem;
  letter-spacing: 0.1em;
  color: #e85d2a;
  margin: 0;
}

.eslogan {
  color: #aaa;
  margin: 0;
}

.prueba {
  margin-top: 2rem;
  padding: 1.5rem;
  border: 1px solid #333;
  border-radius: 12px;
}

button {
  margin: 1rem 0;
  padding: 0.6rem 1.2rem;
  border: none;
  border-radius: 8px;
  background: #e85d2a;
  color: #fff;
  font-size: 1rem;
  cursor: pointer;
}

button:hover {
  background: #ff7a45;
}
</style>