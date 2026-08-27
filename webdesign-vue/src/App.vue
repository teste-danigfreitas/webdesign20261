<script setup>
import { ref } from 'vue'

const contador = ref(0)
const texto = ref('')

</script>

<template>
  <h1>You did it!</h1>
  <p>
    Visit <a href="https://vuejs.org/" target="_blank" rel="noopener">vuejs.org</a> to read the
    documentation
  </p>


<div style="font-family: sans-serif; padding: 2rem; max-width: 400px;">
    <h1>Teste Vue no Codespaces - DANIELLEEEE ------ 🚀</h1>
    
    <div style="margin-bottom: 1.5rem;">
      <p>Contador: <strong>{{ contador }}</strong></p>
      <button @click="contador++" style="padding: 0.5rem 1rem; cursor: pointer;">
        Incrementar
      </button>
      <button @click="contador = 0" style="padding: 0.5rem 1rem; margin-left: 0.5rem;">
        Zerar
      </button>
    </div>

    <hr style="margin: 1.5rem 0; border: none; border-top: 1px solid #ccc;" />

    <div>
      <label for="input-teste" style="display: block; margin-bottom: 0.5rem;">
        Digite algo:
      </label>
      <input 
        id="input-teste"
        v-model="texto" 
        placeholder="Escreva aqui..." 
        style="padding: 0.5rem; width: 100%; box-sizing: border-box;"
      />
      <p style="margin-top: 0.5rem; color: #555;">
        Resultado em tempo real: <strong>{{ texto }}</strong>
      </p>
    </div>
  </div>

</template>

<style scoped></style>
