<script setup>
import { ref } from "vue";

let num = ref(0);
</script>

<template>
  <!-- navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-primary">
    <div class="container-fluid">
      <router-link class="navbar-brand" to="/">
        <img
          src="https://cdn-icons-png.flaticon.com/512/188/188987.png"
          alt="Logo Pikachu"
          width="30"
          height="30"
          class="d-inline-block align-text-top"
        />
        Pokedex Vue
      </router-link>

      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <router-link class="nav-link" aria-current="page" to="/"
              >Home
            </router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/about">Sobre o App </router-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>
  <!-- /navbar -->

  <!-- content -->
  <div class="main">
    <router-view></router-view>
  </div>
  <!-- /content -->

  <!-- footer -->
  <footer class="bg-primary text-light">
    Projeto Pokedex Vue - {{ new Date().getFullYear() }}
  </footer>
  <!-- /footer -->
</template>

<style>
footer {
  position: fixed;
  bottom: 0;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 56px;
}
</style>
