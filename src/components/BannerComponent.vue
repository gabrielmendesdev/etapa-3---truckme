<script setup>
import { onMounted } from 'vue'
import { initFlowbite } from 'flowbite'

onMounted(() => {
    initFlowbite();
})
</script>

<template>
    <div class="flex banner align-middle justify-center">
    </div>
</template>

<style>
.banner {
    width: 100%;
    background-image: url("../assets/truckme.png");
    background-size: cover;
    /* Ajusta a imagem para cobrir completamente o elemento */
    background-position: center center;
    height: calc(100dvh - 70px);
}

@media (max-width: 762px) {
    .banner {
        background-image: url("../assets/truckmemobile.png");
    }
}
</style>