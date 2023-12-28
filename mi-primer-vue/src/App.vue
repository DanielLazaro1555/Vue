<script setup>
const name = 'Vue dinamico'
const stylecolor = 'color:blue'
const arrayColores = ['blue' , 'red' , 'peru']
const activo = false

</script>

<template>
  <h1>Hola {{ name.toUpperCase() }}</h1>
  <h2>{{arrayColores}}</h2>
  <h2 :style="`color:${arrayColores}`">Soy de Perú</h2>
  <h2 v-if="activo">Estoy activo</h2>
  <p v-if="!activo"> Estoy inactivo</p>
</template>

<style>
h1 {
  color: tomato;
}
</style>