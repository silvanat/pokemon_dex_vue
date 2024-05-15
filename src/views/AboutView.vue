<template>
  <div class="container mt-4 text-body-secondary">
    <nav id="navbar-about" class="navbar bg-body-tertiary px-3 mb-3">
      <a class="navbar-brand" href="#">App Pokemon Dex Vue</a>
      <ul class="nav nav-pills">
        <li class="nav-item">
          <a class="nav-link" href="#scroll1">Linguagem</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#scroll2">Recursos</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#scroll3">Objetivo</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#scroll4">GitHub</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#scroll5">Publicação</a>
        </li>
      </ul>
    </nav>
    <div
      data-bs-spy="scroll"
      data-bs-target="#navbar-about"
      data-bs-root-margin="0px 0px -40%"
      data-bs-smooth-scroll="true"
      class="scrollspy-example bg-body-tertiary p-3 rounded-2 mb-5"
      tabindex="0"
    >
      <h4 id="scroll1" class="mt-2">Linguagem</h4>
      <p>Projeto elaborado em Vue 3</p>
      <h4 id="scroll2" class="mt-5">Recursos usados</h4>
      <p>- Bootstrap</p>
      <p>- Vite</p>
      <p>- Animated (CSS)</p>
      <p>- Consumo da API PokeAPI</p>

      <h4 id="scroll3" class="mt-5">Objetivo</h4>
      <p>- Projeto de estudos do Vue 3.</p>
      <h4 id="scroll4" class="mt-5">Github</h4>
      <p>
        O projeto foi publicado no GitHub:
        <a href="https://github.com/silvanat/pokemon_dex_vue" target="_blank"
          >https://github.com/silvanat/pokemon_dex_vue</a
        >
      </p>
      <h4 id="scroll5" class="mt-5">Publicação</h4>
      <p class="mb-5">- Projeto publicado no Netlify:</p>
      <p class="height"></p>
    </div>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
.height {
  height: 400px;
}
</style>
