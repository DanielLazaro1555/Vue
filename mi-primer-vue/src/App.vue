<script setup>
// Definición de variables
const name = 'Vue dinamico'
const stylecolor = 'color:blue'
const arrayColores = ['blue' , 'red' , 'peru']
const activo = null // Puedes agregar un comentario aquí sobre el propósito de la variable
</script>

<template>
  <!-- Usando expresiones y variables -->
  <h1>Hola {{ name.toUpperCase() }}</h1>
  <h2>{{arrayColores}}</h2>
  <h2 :style="`color:${arrayColores}`">Soy de Perú</h2>

  <!-- Usando condicionales -->
  <h2 v-if="activo">Estoy activo</h2>
  <p v-else-if="activo === false">Estoy inactivo</p>
  <p v-else="!activo"> Estoy indeciso</p>
</template>

<style>
/* Estilo CSS para h1 */
h1 {
  color: tomato;
}
</style>
