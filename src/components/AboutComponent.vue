<template>
    <div class="container m-auto">
      <div class="grid grid-section" style="margin-top: 10em">
        <div class="flex align-center flex-col justify-center">
          <h1 class="text-center">Sobre nós</h1>
          <p class="text-start">
            A TruckMe é uma transportadora 100% digital. Trazemos agilidade e
            inteligência em uma solução para melhorar os processos de frete,
            objetivando dinamizar o dia a dia dos nossos clientes e trazer muito
            mais economia.
          </p>
          <br>
          <p class="text-start">
            A TruckMe funciona com uma plataforma digital e aplicativo,
            projetada para conectar, negociar e monitorar as cargas desde a
            solicitação do embarcador até a descarga das cargas...
          </p>
          <br>
          <p class="text-start" :class="{ hidden: isHidden }">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Distinctio saepe
            tenetur repudiandae molestias nobis quaerat repellat. Pariatur excepturi incidunt modi, atque
            distinctio odit? Ullam quasi adipisci sequi laudantium, maiores repellendus? Lorem ipsum dolor, sit
            amet consectetur adipisicing elit. Quasi ratione quas, sapiente necessitatibus facilis maiores rem
            fugit! Provident adipisci dolor impedit, numquam earum in atque accusamus laboriosam, laudantium
            vero sed?</p>
          <br>
          <p class="text-start" :class="{ hidden: isHidden }">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Distinctio saepe
            tenetur repudiandae molestias nobis quaerat repellat.</p>
          <button type="button"
            class="focus:outline-none text-white bg-yellow-400 hover:bg-yellow-500 focus:ring-4 focus:ring-yellow-300 font-medium rounded-lg text-sm px-5 py-2.5 mb-2 dark:focus:ring-yellow-900 w-1/2 mx-auto mt-2"
            @click="toggleVisibility">Saiba Mais...</button>
        </div>
        <div>
          <img src="../assets/sobre_banner.png" alt="imagem de caminhão" class="about-banner rounded-3xl" />
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue';
  
  const isHidden = ref(true);
  
  const toggleVisibility = () => {
    isHidden.value = !isHidden.value;
  };
  </script>
  
  <style scoped>
  .grid-section {
    grid-template-columns: 1fr 1fr;
    gap: 20px;
    margin: 2em;
    margin-top: 4em;
  }
  
  @media (max-width: 992px) {
    .grid-section {
      grid-template-columns: 1fr;
    }
  
    p {
      font-size: 1em;
    }
  }
  </style>
  