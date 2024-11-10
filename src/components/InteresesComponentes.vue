<script setup>
import { ref } from 'vue';
import FondoLava from './FondoLava.vue';
const intereses = ref([
    'Desarrollo de Herramientas Web: Me fascina la creación y optimización de aplicaciones web. Disfruto explorando nuevas tecnologías y frameworks que mejoran el rendimiento y la usabilidad, como Jamstack, GraphQL, y Progressive Web Apps (PWA), siempre buscando formas de implementar soluciones eficientes y escalables.',
    'Comunidades de Programación: Soy un entusiasta de las comunidades de programación y tecnología. Participo en foros y grupos de discusión, donde comparto conocimientos y aprendo de otros desarrolladores. Esta interacción me ayuda a mantenerme al tanto de las últimas tendencias y mejores prácticas en el desarrollo de software.',
    'Automatización y Productividad: Me apasiona la automatización de tareas para mejorar la productividad. Regularmente exploro herramientas como Zapier y servicios en la nube para optimizar procesos repetitivos tanto en el ámbito laboral como en proyectos personales.',
    'Diseño de Experiencia de Usuario (UX): Tengo un interés especial en el diseño centrado en el usuario, buscando siempre mejorar la interacción y experiencia en aplicaciones que desarrollo. Me gusta aprender sobre psicología del usuario y aplicar principios de UX para crear interfaces intuitivas y atractivas.',
    'Gastronomía y Cultura: En mi tiempo libre, disfruto explorar diferentes culturas a través de la gastronomía. Cocinar platos de diferentes partes del mundo me permite relajarme y también entender mejor la diversidad cultural, lo que es valioso cuando trabajo con equipos internacionales.'])

</script>

<template>
    <div class="intereses-contenedor">
        <FondoLava />
        <ul class="contenedor-lista">
            <li class="item" v-for="interes in intereses" :key="interes">
                {{ interes }}
            </li>
        </ul>
    </div>
</template>

<style scoped>
.intereses-contenedor {
    display: flex;
    position: relative;
    margin: 0 auto;
    max-width: 85%;
    padding: 1rem;
}

.contenedor-lista {
    list-style-type: none;
    padding: 1rem;
    margin-bottom: .5rem;
    color: var(--vt-c-white-soft);
    font-size: 1.4rem;
    text-shadow: 3px 3px 6px rgba(0, 0, 0, 1);
}

.item {
    margin-bottom: 1rem;
}
</style>