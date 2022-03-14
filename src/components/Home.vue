<template>
  <div class="layout">
    <div class="header">
      <img src="../assets/logoRick.png" alt="logoRick" class="logoRick" />
      <div class="search">
        <v-icon></v-icon>
        <input type="text" placeholder="Buscar personaje..." />
      </div>
    </div>
    <div class="tabs">
      <nav>
        <a href="">All</a>
        <a href="">Unknown</a>
        <a href="">Female</a>
        <a href="">Male</a>
        <a href="">Genderless</a>
      </nav>
    </div>
    <div class="container">
      <div class="favorite">
        <h2>Mostrar favoritos</h2>
        <button>Fav</button>
      </div>
    </div>
    <div class="footer">
      <img src="../assets/logo.png" alt="logo" />
    </div>
  </div>
</template>
<script>
export default {
  name: "Home",
};
</script>
<style scoped>
.header {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 455px;
  background-image: url(../assets/fondoWelcome.png);
  background-color: black;
  background-size: cover;
  background-position: center;
}

.logoRick {
  width: 347px;
  height: 122px;
}
</style>