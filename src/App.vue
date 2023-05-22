<script setup>
  import {livros} from '@/_data/livros'
</script>
<template>
  <h1>Minha livraria</h1>
  <div class="livros">
    <div class="card-livro" v-bind:on-beforeinput="livro in livros" :key="livro.id">
      <img :src="livro.cover" class="livro-capa"/>
      <p class="livro-titulo">{{livro.title}}</p>
      <p class="livro-titulo">{{livro.author}}</p>
      <p class="livro-titulo">{{livro.price}}</p>
    </div>
  </div>
</template>

<style scoped>

</style>
