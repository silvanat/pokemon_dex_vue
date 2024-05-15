<script setup>
const pokemon = defineProps(["name", "urlBaseSvg"]);
const indice = pokemon.url;
</script>

<template>
  <div class="col-6">
    <div class="card mb-3 p-2 cardListPokemon">
      <p class="text-center">{{ pokemon.name }}</p>
      <img
        :src="urlBaseSvg"
        class="card-img-top"
        :alt="pokemon.name"
        height="80"
      />
    </div>
  </div>
</template>

<style scoped>
.cardListPokemon {
  background: rgb(63, 74, 251);
  background: radial-gradient(
    circle,
    rgba(63, 74, 251, 0.3) 0%,
    rgba(70, 252, 199, 0.02) 100%
  );
  cursor: pointer;
}

.cardListPokemon:hover {
  background: rgb(63, 74, 251);
  background: radial-gradient(
    circle,
    rgba(63, 74, 251, 0.4) 0%,
    rgba(70, 252, 199, 0.06) 100%
  );
}

.cardListPokemon img:hover {
  padding: 0.1rem;
  opacity: 0.9;
}
</style>
