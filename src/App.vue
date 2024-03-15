<script setup>

</script>

<template>
  <div class="fondo">
    <header>
      <div class="contenedor">
        <div class="menu">
          <img id="logo" src="./logo.png" alt="">
          <nav>
            <ul class="lista">
              <li>Inicio</li>
              <li>Sobre nosotros</li>
              <li>Noticias</li>
              <li>Contacto</li>
            </ul>
          </nav>
          <div class="telefonoDiv">
            <p class="telefono"> Contacto: 674956320</p>
          </div>
        </div>
      </div>
    </header>
    <main>
      <div class="noticia1">
        <img id="imagen1" src="./imagen1.jpg" alt="">
        <p id="texto1">No deja de ser paradójico: justo ahora que el futuro de las películas de superhéroes es más
          impredecible que nunca, la última superheroína de Marvel es una pitonisa. El nuevo estreno de la hasta ahora
          prolífica y rentable factoría, Madame Web, se enfrenta a una bola de cristal opaca y difícil de descifrar ante
          el evidente declive del género que ha copado hasta la extenuación las pantallas de cine de los últimos años.
        </p>
      </div>

      <div class="noticia2">

        <p id="texto2">Los gamers que siguen disfrutando de Marvel´s Spider-Man 2 están a la espera de lo que será el
          nuevo Modo New Game Plus. Y sobre esto y más llegan novedades desde PlayStation.

          Esta nueva modalidad, además de nuevo contenido y otros extras, estarán llegando al título desde el próximo 7
          de marzo gracias a una actualización.

          Para ser más exactos, este nuevo update añadirá la posibilidad de poder volver a jugar misiones específicas,
          además de ofrecer una dificultad con nivel, nuevos objetos desbloqueables y más.
        </p>
        <img id="imagen2" src="./fondo.jpg" alt="">
      </div>
      <div class="video">

        <p id="texto2">La última entrega de Spider-Man es, un verdadero evento, como era de esperar. Su predecesora,
          'Spider-Man: Un nuevo universo' fue toda una revolución en 2018. Con razón se llevó el Oscar a Mejor Película
          de Animación en los Óscar 2019.

          Aquí el cargo de trepamuros caía en un adolescente llamado Miles Morales, en un mundo en el que Peter Parker
          ha fallecido. Cuando el líder mafioso Wilson Fisk construye el "Super Colisionador" trae con él a una versión
          alternativa de Peter Parker que instruirá a Miles en cómo ser el mejor Spider-Man. Pero no será el único
          'Spidey' en entrar a este universo: de hecho conocerá a 4 versiones alternas que aparecerán y buscarán
          regresar a su mundo de procedencia antes de que toda la realidad colapse.
        </p>
        <video width="360" height="640" autoplay muted>
          <source src="./video.mp4">
        </video>
      </div>

      <div class="video">

        <h3>Escucha la auténtica cancion de Spiderman</h3>
        <audio autoplay controls>
          <source src="./audio1.mp3" type="audio/mp3">
        </audio>
      </div>

    </main>

  </div>
  <footer>
    <div class="pie">
      <p id="direccion">C/Embajadores 69</p>
      <p id="copi">copyright</p>
      <p id="redes">Siguenos en nuestras RRSS</p>
    </div>
  </footer>

</template>

<style scoped>
.pie {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  width: 100%;
  background-color: rgb(147, 33, 33, 0.699);
  height: 64px;
}

.telefono {
  margin-right: 15vh;
}

#redes {
  margin-right: 15vh;
}

#direccion {
  margin-left: 15vh;
}

.fondo {
  background-image: url(./fondo2.jpg);
  background-size: 100%;

}

.noticia1 {
  display: flex;
  flex-wrap: wrap;
  gap: 20%;
  border: 1px solid #6b2d2d;
  padding: 8px;
  text-align: left;
  background-color: rgba(59, 13, 13, 0.699);
  color: #ddd;
  width: 80%;
  margin-top: 5%;
  margin-left: 10%;
  border-radius: 10px;

}


.noticia2 {
  display: grid;
  grid-template-areas: "texto2 texto2"
    "imagen2 imagen2";
  grid-template-rows: repeat(12, auto);
  text-align: right;
  gap: 20%;
  border: 1px solid #6b2d2d;
  padding: 8px;
  text-align: left;
  background-color: rgba(59, 13, 13, 0.699);
  color: #ddd;
  width: 80%;
  margin-top: 5%;
  margin-left: 10%;
  border-radius: 10px;

}

.video {
  display: flex;
  flex-wrap: wrap;
  gap: 20%;
  border: 1px solid #6b2d2d;
  padding: 8px;
  text-align: left;
  background-color: rgba(59, 13, 13, 0.699);
  color: #ddd;
  width: 80%;
  margin-top: 5%;
  margin-left: 10%;
  border-radius: 10px;

}

#texto1 {
  width: 50vh;
}

#texto2 {
  width: 50vh;
  margin-left: 15vh;
  margin-top: 25vh;
}

#imagen1 {
  margin-left: 8%;
  scale: 75%;
}

#imagen2 {
  margin-left: 15%;
  scale: 65%;

}


.menu {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  width: 100%;
  background-color: rgb(147, 33, 33, 0.699);
  height: 64px;
}

.lista {
  list-style: none;

}

li {
  float: left;
  margin-right: 10px;
  color: azure;
}

#logo {
  width: 15vh;
}

@media (max-width: 767px) {
  template {
    width: 80%;
  }

  .noticia1 {
    scale: 80%
  }

  .noticia2 {
    scale: 80%;
    display: grid;
    grid-template-areas: "texto2  "
      "imagen2 ";


  }
  #imagen2{
    width: 80%;
    margin-bottom: 50%;
  }
  #texto2{
    height: 50%;
  }
  #direccion{
    scale: 80%;
  }
  #redes{
    scale: 80%;
  }
  #copi{
    scale: 80%;
  }

  .video {
    scale: 80%
  }

  .contenedor {
    scale: 80%
  }
  nav {
    scale: 80%
  }

  .pie {
    display: flex;
  flex-wrap: wrap;
    justify-content: space-between;
    scale: 100%;

  }

}

@media (min-width: 768px) and (max-width: 991px) {

  template {
    width: 90%;
  }

  .noticia1 {
    scale: 90%
  }

  .noticia2 {
    scale: 90%
  }

  .video {
    scale: 90%
  }

  .contenedor {
    scale: 90%
  }

  .pie {
    scale: 90%
  }

}


@media (min-width: 992px) {

  template {
    width: 100%;
  }

  .noticia1 {
    scale: 100%
  }

  .noticia2 {
    scale: 100%
  }

  .video {
    scale: 100%
  }

  .contenedor {
    scale: 100%
  }

  .pie {
    scale: 100%
  }
}
</style>
