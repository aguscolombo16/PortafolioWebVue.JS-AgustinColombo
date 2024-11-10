<script setup>
const title = "Agustin Colombo"
const descripcion ="Tecnico Universitario en Programacion - UTN"
const residencia = "San Rafael ,Mendoza, Argentina"
const presentacion = "Hola , Bienvenido a mi portafolio de proyectos, Soy un desarrollador web con experiencia en el desarrollo de aplicaciones web y moviles."
const redesSociales =[
    {id: 1, name: "linkedin", src:"/src/assets/icons/linkedin_icon.svg", url: "https://www.linkedin.com/in/agust%C3%ADn-colombo-9611a522a/ "},
    {id: 2, name: "Instagram", src:"/src/assets/icons/instagram_icon.svg", url: "https://www.instagram.com/aguscolombo16/?hl=es"},
    {id: 3, name: "github", src:"/src/assets/icons/github_icon.svg", url: "https://github.com/aguscolombo16"},
    {id: 4, name: "curriculum", src:"/src/assets/icons/cv_resume_icon.svg", url: "https://www.canva.com/design/DAGKAr0QjDU/y9DWANo0F286Eiz_9BANXA/view?utm_content=DAGKAr0QjDU&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink&mode=preview"},
];
const telefono = "+54 9 2604-222363";
</script>

<template>
    <section class="datos-personales">
        <div class="card">
            <h1>{{ title }}</h1>
            <h2>{{ descripcion }}</h2>
            <p>{{ presentacion }}</p>
            <ul class="container-lista">
                <li v-for="red in redesSociales" :key="red.id">
                    <a :href="red.url"><img class="icon-redsocial" :src="red.src" width="35rem" :alt="red.name"></a>
                </li>
            </ul>
            <h3> Mi telefono personal: {{ telefono }}</h3>
            <h4>{{ residencia }}</h4>
        </div>
    </section>
</template>
<style scoped>
h1{
    font-size: 2.5rem;
}
p{
    font-size: 1.2rem;
    font-weight: 600;
    margin-bottom:1rem;
}

.card {
    background-color:rgb(173, 54, 54);
    border-radius: 10px;
    padding: 10px;
    margin: 1opx;
    text-align: center;
}

.container-lista {
    display: flex;
    justify-content: center;
    list-style: none;
    padding: 0;
    margin: 0;
    text-align: center;
}

.icon-redsocial {
    align-items:center;
    background-color:rgb(255, 240, 240); ;
    border-radius: 50%;
    padding: 2px;
    margin:5px;
    box-shadow: 0 0 5px rgba(0, 0, 0, 0.934);
}

.icon-redsocial:hover{
    background-color:rgb(0, 0, 0) ;
    box-shadow: 0 0 5px rgba(251,249,249,0.934);
}
h3 {
    font-size: 1.2rem;
    font-weight: 600;
}
</style>