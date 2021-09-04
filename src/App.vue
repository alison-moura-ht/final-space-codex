<template>
  <div class="bg-gray-800 p-2 lg:p-20">
    <img width="300" alt="Vue logo" src="./assets/Final_Space_Logo.png" class="mx-auto mb-10 mt-20 lg:mt-0" />
    <characters-list></characters-list>
  </div>
  <footer class="bg-gray-900 px-10 lg:px-20 py-10 text-sm">
    <p class="text-white">
      An example of frontend aplication consuming
      <a
        href="https://finalspaceapi.com/"
        class="text-blue-500 font-bold"
      >Final Space API</a>.
      Developed by
      <a
        href="https://fabricadeprogramador.com.br"
        class="text-blue-500 font-bold"
      >Fábrica de Programador</a>.
    </p>
  </footer>
</template>

<script setup>
import CharactersList from './components/CharactersList.vue'
</script>

