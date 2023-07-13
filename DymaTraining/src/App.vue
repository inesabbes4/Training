<template>
  <h1 v-bind="obj">Bonjour {{ `${name} je concatène` }} </h1>
  <input :type="getType()">
</template>

<script setup lang="ts">
import { VueElement, createApp } from 'vue';


  const h1title = 'montitre2'
  const h1id = 'monid2'
  const name = 'Dyma'

  const obj = {
    'class' : h1title,
    'id' : h1id
  }

  function getType() {
    return 'date'
  }

  const vue = createApp({});

</script>

<style></style>