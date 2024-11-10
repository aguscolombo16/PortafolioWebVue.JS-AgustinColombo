<script setup>
import icono1 from '/src/assets/icons/ventas.svg';
import icono2 from '/src/assets/icons/ecomerce.svg';
import icono3 from '/src/assets/icons/configuracion.svg';
import icono4 from '/src/assets/icons/uiux.svg';
import icono5 from '/src/assets/icons/watch.svg';

import { ref } from 'vue';
const titulo = 'Desarrollador Full Stack';
const fecha = 'Desde Enero 2022 / Julio 2024';
const experiencias = ref([
    { id: 1, parrafo: ' Optimización de rendimiento: "Desarrollé e implementé mejoras en la estructura de la base de datos y en el código backend, reduciendo los tiempos de carga de la aplicación en un 40%, lo que mejoró la experiencia del usuario y aumentó la retención en un 20%.',src: icono1 },
    { id: 2, parrafo: 'Integración de API: "Lideré la integración de varias APIs de terceros (como servicios de pago y mensajería), mejorando la funcionalidad de la plataforma y reduciendo el tiempo de procesamiento de transacciones en un 30%.', src: icono2},
    { id: 3, parrafo: 'Automatización de procesos: "Diseñé y desarrollé scripts automatizados que redujeron los tiempos de compilación y despliegue en un 50%, lo que permitió que el equipo de desarrollo se enfocara más en la implementación de nuevas funcionalidades',src: icono3 },
    { id: 4, parrafo: 'Mejora de seguridad: "Implementé protocolos de seguridad avanzados y prácticas de desarrollo seguro, lo que resultó en la identificación y resolución de vulnerabilidades críticas, reduciendo el riesgo de ataques en un 80%.',src: icono4 },
    { id: 5, parrafo: 'Experiencia de usuario: "Rediseñé la interfaz de usuario de una aplicación web, mejorando la navegación y accesibilidad, lo que resultó en un incremento del 15% en la interacción de los usuarios.', src: icono5},
]);
</script>

<template>
    <div class="card">
        <h3 class="titulo">{{ titulo.toLocaleUpperCase() }}</h3>
        <p class="fecha">{{ fecha }}</p>
        <ul class="listado">
            <li class="item" v-for="experencia in experiencias" :key="experencia.id">
                <img class="imagen-svg" :src="experencia.src" width="45rem" :alt="experencia.parrafo">
                <p>{{ experencia.parrafo }}</p>
            </li>
        </ul>
    </div>
</template>

<style scoped>
.card {
    display: flex;
    flex-direction: column;
    padding: 2rem;
    background-color: rgb(28, 41, 52);
    border-radius: 15px;
}

.titulo {
    font-size: 1.5rem;
    color: coral;
}

.fecha {
    font-size: 1rem;
    color: burlywood;
    margin-bottom: 1rem;
}

.listado {
    display: flex;
    flex-direction: column;
}

.item {
    align-items: center;
    display: flex;
    padding: 1rem;
    gap: 1.5rem;
}
</style>