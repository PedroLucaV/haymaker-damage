<script setup>
import { ref } from 'vue'
import './App.css'

const msg = ref(0)
</script>

<template>
  <div class='container'>
    <header class='header'>
      <h1>Sett</h1>
      <h2>
        Haymaker Damage Calculator
      </h2>
    </header>
    <main class='main'>
      <h1 class='ousadia'>Ousadia {{ (msg / 2).toFixed(0) }}</h1>
      <h2>Dano Verdadeiro: {{ (80 + ((msg / 2) * 0.26)).toFixed(0) }}</h2>
      <span>
        <label for="vida">Quanto de HP: </label>
        <input type="number" v-model="msg" name="vida"/>
      </span>
    </main>
  </div>
</template> 