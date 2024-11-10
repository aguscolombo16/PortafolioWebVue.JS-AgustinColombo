<script setup>
import NavBar from './components/NavBar.vue';
import DatosPersonales from './components/DatosPersonales.vue';
import EDUCACION1 from './components/EDUCACION1.vue';
import ExperienciaComponente from './components/ExperienciaComponente.vue';
import ProyectosComponentes from './components/ProyectosComponentes.vue';
import HabilidadesComponentes from './components/HabilidadesComponentes.vue';
import InteresesComponentes from './components/InteresesComponentes.vue';
</script>

<template>
    <header id="top">
        <!--Barra de Navegacion-->
        <NavBar />
        <!--Componente Datos Personales-->
        <DatosPersonales />
    </header>
    <main>
        <!--el estilo css de section se encuentra en base.css-->
        <section id="educacion">
            <h2>Educación - Cursos</h2>
            <!--Componente Educación-->
            <EDUCACION1 />
        </section>
        <section id="experiencia">
            <h2>Educacion</h2>
            <!--Componente Experiencia-->
            <ExperienciaComponente />
        </section>
        <section id="proyectos">
            <h2>Proyectos</h2>
            <!--Componente Proyectos-->
            <ProyectosComponentes />
        </section>
        <section id="habilidades">
            <!--Componente Habilidades-->
            <h2>Habilidades</h2>
            <HabilidadesComponentes />
        </section>
        <section id="intereses">
            <!--Componente Intereses-->
            <h2>Intereses</h2>
            <InteresesComponentes />
        </section>
    </main>
    <footer>
        <a href="#top">Inicio</a>
        <p>Agustin Colombo Portafolio web</p>
    </footer>
</template>

<style scoped>
footer {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 2rem;
    font-size: 1.3rem;
}
</style>

