<template>
  <div class="layout">
    <div class="layoutMidle">
      <img
        src="../assets/logo.png"
        alt="logoSuazo"
        class="logoSuazo"
      />
      <img src="../assets/logoRick.png" alt="logoRick" class="rickMarty" />
      <h1>Bienvenido a Rick and Marty</h1>
      <p>
        En esta prueba, evaluaremos su capacidad para construir la aplicación
        mediante el análisis de código y la reproducción del siguiente diseño.
      </p>
      <button class="button" @click="goHome">Continuar</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  data() {
    return {
    }
  },
  methods: {
      goHome() {
        this.$router.replace({
         path: '/home' 
        })
      }
    },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

body html {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
.layout {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 1024px;
  background-image: url("../assets/fondoWelcome.png");
  background-repeat: no-repeat;
  background-color: black;
  min-width: 1440px;
}

.layoutMidle {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.logoSuazo {
  width: 135px;
  height: 50px;
}

.rickMarty {
  width: 664px;
  height: 233px;
}

.button {
  widows: 120px;
  height: 44px;
  border-radius: 25pX;
  padding: 11px 20px 11px 20px;
  background-color: #11555F;
  color: white;
}
</style>
