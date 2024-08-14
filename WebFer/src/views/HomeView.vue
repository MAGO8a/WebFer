<script setup>
import Header from '@/components/Header.vue'
import SearchIcon from '../components/SearchIcon.vue'
import AccountIcon from '@/components/AccountIcon.vue'
import HelpIcon from '@/components/HelpIcon.vue'
import IdeaIcon from '@/components/IdeaIcon.vue'
</script>

<template>
  <div class="back">
    <div class="app-container">
      <Header class="head" />

      <div style="padding-top: 60px">
        <div class="container">
          <v-card loading variant="elevated" class="Card">
            <div style="margin: 20px">
              <div
                style="
                  display: flex;
                  flex-direction: row; /* Cambia de columna a fila */
                  justify-content: center;
                  align-items: center;
                  width: 100%;
                "
              >
                <AccountIcon size="40" />
                <h2>Quienes somos</h2>
              </div>
              <a-divider style="background-color: #f4d03f" />
              <p style="margin: 10px">
                Somos un equipo de ingenieros y operarios que trabajamos con el fin de construir un
                hogar confortable y estético. Nos caracteriza la profesionalidad y el cumplimiento
                de los tiempos establecidos
              </p>
            </div>
          </v-card>
        </div>

        <div class="container">
          <v-card loading variant="elevated" class="Card">
            <div style="margin: 20px">
              <div
                style="
                  display: flex;
                  flex-direction: row; /* Cambia de columna a fila */
                  justify-content: center;
                  align-items: center;
                  width: 100%;
                "
              >
                <HelpIcon size="40" />

                <h2>Podemos serte de ayuda</h2>
              </div>
              <a-divider style="background-color: #f4d03f" />
              <p style="margin: 10px">
                Ofrecemos servicios de construcción y diseño de interiores. En nuestro Marketplace
                encontrarás productos para el hogar importados y nacionales de las mejores marcas
                del pais. Contatca con nosotros para ayudarte a construir el hogar perfecto
              </p>
              <div
                style="
                  display: flex;
                  flex-direction: row; /* Cambia de columna a fila */
                  justify-content: center;
                  align-items: center;
                  width: 100%;
                  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans',
                    Arial, sans-serif;
                "
              >
                <v-btn style="margin: 10px; background-color: #f4d03f">Contactanos!</v-btn>
              </div>
            </div>
          </v-card>
        </div>

        <div class="container">
          <v-card loading variant="elevated" class="Card">
            <div style="margin: 20px">
              <div
                style="
                  display: flex;
                  flex-direction: row; /* Cambia de columna a fila */
                  justify-content: center;
                  align-items: center;
                  width: 100%;
                "
              >
                <IdeaIcon size="40" />
                <h2>Inspírate</h2>
              </div>
              <a-divider style="background-color: #f4d03f" />

              <v-carousel show-arrows="hover">
                <v-carousel-item
                  src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
                  cover
                ></v-carousel-item>

                <v-carousel-item
                  src="https://cdn.vuetifyjs.com/images/cards/hotel.jpg"
                  cover
                ></v-carousel-item>

                <v-carousel-item
                  src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                  cover
                ></v-carousel-item>
              </v-carousel>

              <p style="margin: 10px">
                Nuestros trabajps pueden ser una buena fuente de ideas para llevar a cabo en la
                comodidad de tu casa, negocio o espacio que desees darle una nueva vista
              </p>
              <div
                style="
                  display: flex;
                  flex-direction: row; /* Cambia de columna a fila */
                  justify-content: center;
                  align-items: center;
                  width: 100%;
                  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans',
                    Arial, sans-serif;
                "
              >
                <v-btn style="margin: 10px; background-color: #f4d03f">Catálogo</v-btn>
              </div>
            </div>
          </v-card>
        </div>

        <div class="container">
          <v-card loading variant="elevated" class="Card">
            <div style="margin: 20px">
              <div
                style="
                  display: flex;
                  flex-direction: row; /* Cambia de columna a fila */
                  justify-content: center;
                  align-items: center;
                  width: 100%;
                "
              >
                <SearchIcon size="40" />
                <h2>¿Quienes somos?</h2>
              </div>
              <a-divider />
              <p style="margin: 10px">
                Somos un equipo de ingenieros y operarios que trabajamos con el fin de construir un
                hogar confortable y estético. Nos caracteriza la profesionalidad y el cumplimiento
                de los tiempos establecidos
              </p>
            </div>
          </v-card>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.app-container {
  width: 100vw; /* Asegura que ocupe todo el ancho de la ventana */
  min-height: 100vh; /* Asegura que ocupe al menos todo el alto de la ventana */
  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial,
    sans-serif;
}

.back {
  background-image: url(../assets/60129-casas.jpg);
  background-position: center; /* Centra la imagen */
  background-repeat: no-repeat; /* Evita que la imagen se repita */
  background-size: cover; /* Ajusta el tamaño de la imagen para cubrir completamente el área disponible sin distorsionarla */
  background-attachment: fixed;
  height: 100%;
}

.container {
  display: flex;
  flex-wrap: wrap; /* Permite que las tarjetas se envuelvan a la siguiente línea */
  gap: 20px; /* Ajusta el espacio entre las tarjetas */
}
.Card {
  width: 50%;
  font-size: 20px;
  border: 2px solid #f4d03f;
  margin: auto; /* Centra el v-card horizontalmente */
  border-radius: 10px;
  margin-top: 120px;
}

.Card h2 {
  font-size: 30px;
  margin-left: 10px;
}

.head {
  border-radius: 10px;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1000; /* Asegura que el header esté por encima de otros contenidos */
}
</style>
