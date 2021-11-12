<template>
    <div style="textAlign: center; backgroundColor: white; width: 100%; height: 100%;">
        <p style="color: black; marginTop: 5px">contenido de prueba con un div de fondo blanco</p><br><br>
        <button @click="funcionPrueba2">abrir una ventana con fondo verde</button>
    </div>
</template>

<script setup lang="ts">
import Glayout from "Glayout.vue";
import { ref } from "vue";
import { prefinedLayouts } from "../ts/predefined-layouts";

const GLayoutRoot = ref<null | HTMLElement>(null);

const funcionPrueba2 = () => {
    console.log("funcion prueba 2 iniciando desde la ventana de fondo blanco");
    if (!GLayoutRoot.value) return;
    GLayoutRoot.value.addGLComponent("ContenidoPrueba2", "color verde");
};
</script>