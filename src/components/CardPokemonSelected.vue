<script setup>
const pokemon = defineProps(["name", "xp", "height", "img", "loading"]);
</script>

<template>
  <div
    class="card card-pokemon-selected"
    :class="loading ? '' : 'animate__animated animate__flipInY'"
  >
    <img
      v-if="pokemon.name"
      :src="pokemon.img"
      class="card-img-top pt-5"
      :alt="pokemon.name"
    />
    <img
      v-else
      src="../assets/egg_pokemon.svg"
      class="card-img-top pt-5"
      alt="Ovo Pokemon"
    />
    <div class="card-body">
      <h5 class="card-title text-center">
        {{ pokemon.name || " - " }}
      </h5>
      <hr class="pt-2" />
      <div class="row">
        <section class="col">
          <strong>XP:</strong>
          <span class="ms-1">{{ pokemon.xp || " - " }}</span>
        </section>
        <section class="col">
          <strong>Altura:</strong>
          <span class="ms-1">{{ pokemon.height || " - " }}</span>
        </section>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card-pokemon-selected {
  background: rgb(154, 162, 247);
  background: radial-gradient(
    circle,
    rgba(55, 67, 233, 0.3) 0%,
    rgba(70, 252, 199, 0.02) 100%
  );
  height: 75vh;
}
.card-pokemon-selected img {
  height: 250px;
}
@media (max-width: 768px) {
  .card-pokemon-selected {
    height: 260px;
    margin: 0 auto 10px;
    width: 40%;
  }
  .card-pokemon-selected img {
    height: 130px;
  }
}
</style>
