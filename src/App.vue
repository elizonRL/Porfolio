<template class=" contem">
  <div class="portfolio">
    <header>
      <!-- Aquí puedes agregar el encabezado de tu porfolio -->
      <div>
        <h1>Mi Portafolio</h1>
      </div>
      <div>
        <nav>
          <ul>
            <li><a href="#about">Acerca de mí</a></li>
            <li><a href="#projects">Proyectos</a></li>
            <li><a href="#contact">Contacto</a></li>
          </ul>
        </nav>
      </div>
    </header>

    <main>
      <!-- Aquí puedes agregar el contenido principal de tu porfolio -->
      <section class="perfil">
        <div class="imagenPerfil">
          <img src="./assets/perfil.jpg" alt="Imagen de perfil de ELIZON Rodriguez" />
        </div>
        <div class="infoPersonal">
          <h2>Elizon Rodriguez Liriano</h2>
          <p>Desarrollador Frontend</p>
        </div>
        <div class="redesSociales">
          <a href="www.linkedin.com/in/elizon-rodriguez-91ab21236" target="_blank">
            <IconLinkedin class="icons" />
          </a>
          <a href="">
            <IconXtwitter class="icons" />
          </a>
          <a href="">
            <IconGithub class="icons" />
          </a>

        </div>
      </section>
      <section class="about">
        <h3>Acerca de mí</h3>
        <p>Soy un programador web titulado de la Universidad Autónoma de Santo Domingo. Me gradué en el año 2023 de
          licenciatura en informática.</p>
        <p>Desde que era pequeño, siempre me han interesado las computadoras y la tecnología. Me encantaba aprender sobre
          cómo funcionaban las cosas y cómo podía crearlas yo mismo.</p>
        <p>Cuando entré a la universidad, sabía que quería estudiar informática. Me parecía una carrera emocionante y
          desafiante, y sabía que me permitiría trabajar en una amplia gama de campos relacionados con la tecnología.</p>
        <p>Durante mis estudios, aprendí sobre una amplia gama de temas relacionados con la informática, incluyendo la
          programación, el análisis de datos, la seguridad informática y más. También tuve la oportunidad de participar en
          proyectos de informática, lo que me ayudó a desarrollar mis habilidades prácticas.</p>
        <p>En la universidad, aprendí a programar en Java, C, C ++ y Python. También aprendí sobre estructuras de datos,
          algoritmos y
          diseño de software. En el trascurso, comencé a aprender desarrollo web por mi cuenta.</p>
        <p>Me encanta aprender cosas nuevas y siempre estoy buscando formas de mejorar mis habilidades. Me encanta
          trabajar en equipo y aprender de los demás.</p>
      </section>
      <section class="proyectos">
        <div>
          <h3>Proyectos</h3>
          <p>Estos son algunos de los proyectos en los que he trabajado:</p>
        </div>
        <div>
          
        </div>
      </section>
    </main>

    <footer>
      <!-- Aquí puedes agregar el pie de página de tu porfolio -->
    </footer>
  </div>
</template>

<script>

import IconLinkedin from './components/icons/IconLinkedin.vue';
import IconXtwitter from './components/icons/IconXtwitter.vue';
import IconGithub from './components/icons/iconGithub.vue';

export default {
  name: 'App ',
  components: {
    IconLinkedin,
    IconXtwitter,
    IconGithub
  }


}
</script>

<style>
/* Aquí puedes agregar estilos CSS para tu porfolio */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: ' Poppins', sans-serif;
}

.contem {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: #f5f5f5;
  font-family: 'Roboto', sans-serif;
  font-size: 16px;
  color: #333;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.contem header {
  width: 100%;
  height: 60px;
  background-color: #1f1e1e;
  display: flex;
  justify-content: space-around;
  align-items: center;
  padding: 0 20px;
  box-sizing: border-box;
}

.perfil {
  display: grid;
  grid-template-columns: 1fr 3fr 1fr;
  justify-content: center;
  align-items: center;
  background-image: url(../public/img/fondo.jpg);
  font-family: 'Popins', sans-serif;
  font-size: 16px;
  color: #fff;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  grid-template-areas: "imagen info info redes";
  border-radius: 3px;
  border-bottom: solid 7px var(--green-color);
}

.imagenPerfil {
  display: flex;
  justify-content: center;
  align-items: center;
  grid-area: imagen;
}

.redesSociales {
  columns: 1fr 1fr 1fr;
  grid-area: redes/-1;
  grid-row: -1/-1;
  padding-left: 5px;
}

.infoPersonal {
  text-shadow: 6px 3px 4px #000;
  grid-area: info;
  gap: 10px;
}

.icons {
  width: 30px;
  height: 30px;
  margin: 0 10px;
  transition: all 0.3s ease-in-out;
}

.icons:hover {
  transform: scale(1.4);
}

.infoPersonal h2 {
  font-size: 30px;
  font-weight: 700;
}

.about {
  display: flex;
  flex-direction: column;
  min-height: 400px;
  background-color: #1f1e1e;
  font-family: 'Roboto', sans-serif;
  font-size: 16px;
  color: #FFF;
  margin: 10px 0;
  padding: 0;
  box-sizing: border-box;
  border-radius: 5px;
  border-bottom: solid 7px var(--green-color);
}

.about h3 {
  font-size: 23px;
  font-weight: 700;
  text-align: center;
  margin: 10px 0;
}

.about p {
  padding: 0 5px;
  margin: 3px 5px;
  font-size: 16px;
  font-weight: 500;
  line-height: 1.6;
  word-spacing: 2px;
}

.proyectos {
  display: flex;
  flex-direction: column;
  min-height: 400px;
  background-color: #1f1e1e;
  font-family: 'Roboto', sans-serif;
  font-size: 16px;
  color: #FFF;
  margin: 10px 0;
  padding: 0;
  box-sizing: border-box;
  border-radius: 5px;
  border-bottom: solid 3px var(--green-color);
}

.proyectos h3 {
  font-size: 23px;
  font-weight: 700;
  text-align: center;
  margin: 10px 0;
}


/* Aquí puedes agregar estilos para las Eriquetas*/
header h1 {
  font-size: 32px;
  font-weight: 700;
  color: #fff;
  border-bottom: solid 5px var(--green-color);
  border-radius: 5px;
}

nav {
  background-color: #2b2929;
  padding: 10px;
  margin: 10px;
}

ul {
  list-style: none;
  display: flex;
}

ul li {
  margin: 0 10px;

}

li a:hover {
  background-color: var(--green-color);
  color: #fff;
  padding: 10px;
  border-radius: 3px;
}

img {
  width: 200px;
  height: 200px;
  border-radius: 50%;
  margin: 20px 0;
}</style>
