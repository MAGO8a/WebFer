<template>
  <div>

    <a-card class="Card" :bordered="true">
      <SearchIcon/>
      <h2>¿Quienes somos?</h2>
      <a-divider />
      <p>
        Somos un equipo de ingenieros y operarios que trabajamos con el fin de construir un hogar
        confortable y estético. Nos caracteriza la profesionalidad y el cumplimiento de los tiempos
        establecidos
      </p>
    </a-card>
  </div>
</template>

<script>
import SearchIcon from './SearchIcon.vue';
</script>

<style scoped>
.Card {
  width: 50%;
  font-size: 20px;
}

.Card h2 {
  font-size: 30px;
}
</style>
