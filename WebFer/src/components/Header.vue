<template>
  <v-toolbar density="prominent" :elevation="8" :absolute="false" class="toolbar-custom">
    <div
      style="
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 100%;
        font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial,
          sans-serif;
      "
    >
      <div
        style="
          display: flex;
          flex-direction: row; /* Cambia de columna a fila */
          justify-content: center;
          align-items: center;
          width: 100%;
        "
      >
        <HeadIcon size="40"/>
        <span class="text-h5">
          <h1>Concepto</h1>
        </span>
      </div>
      <span class="text-subtitle-1">Diseño, construcción y mobiliario</span>
    </div>
  </v-toolbar>
</template>

<style scoped>
.text-h5 {
  display: flex;
  text-align: center;
  margin: 10px;
  font-size: 100px;
}

.toolbar-custom {
  max-width: 90%; /* Limita el ancho máximo del toolbar a 90% del ancho de la pantalla */
  margin: auto; /* Ajusta el margen superior a 20px, manteniendo el centrado horizontal y el margen inferior predeterminado */
  padding: 0 10px; /* Agrega un poco de relleno interno para darle un poco de espacio al contenido */
}

.text-subtitle-1 {
  text-align: center;
  margin-top: auto; /* Empuja hacia abajo el texto del subtítulo para centrarlo verticalmente */
}
</style>

<script>
import HeadIcon from './HeadIcon.vue'
</script>
