<script setup>
const name = 'Vue dinamico'
const stylecolor = 'color:blue'
const arrayColores = ['blue' , 'red' , 'peru']
const activo = null

</script>

<template>
  <h1>Hola {{ name.toUpperCase() }}</h1>
  <h2>{{arrayColores}}</h2>
  <h2 :style="`color:${arrayColores}`">Soy de Perú</h2>
  <h2 v-if="activo">Estoy activo</h2>
  <p v-else-if="activo === false">Estoy inactivo</p>
  <p v-else="!activo"> Estoy indeciso</p>
</template>

<style>
h1 {
  color: tomato;
}
</style>