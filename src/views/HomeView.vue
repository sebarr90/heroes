<template>
  <v-app>
    <!-- Barra de navegación -->
    <v-app-bar app color="blue darken-4" dark>
      <v-btn icon @click="$router.push('/')">
        <v-icon>mdi-home</v-icon>
      </v-btn>
      <v-toolbar-title>Heroes of the Storm</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn color="orange darken-3" @click="$router.push('/heroes')">Ver Héroes</v-btn>
    </v-app-bar>

    <!-- Contenido principal -->
    <v-main>
      <div class="home-background">
        <v-container class="text-center d-flex flex-column justify-center align-center fill-height">
          <h1 class="display-2 white--text font-weight-bold mb-4">Desafía las expectativas de los MOBA</h1>
          <p class="white--text subtitle-1 mb-5">
            Épicos héroes y acción sin cesar en múltiples campos de batalla
          </p>
          <v-btn large color="orange darken-3" @click="$router.push('/heroes')">Ver Héroes</v-btn>
        </v-container>
      </div>
    </v-main>

    <!-- Pie de página -->
    <v-footer app color="blue darken-4">
      <span class="white--text">&copy; Bienvenido a vuetify 2021 —</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: "HomeView",
};
</script>

<style scoped>
.home-background {
  background: url('https://static.heroesofthestorm.com/heroes/yrel/skins/light-of-hope-800.jpg') no-repeat center center fixed;
  background-size:cover;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;

}

.white--text {
  text-shadow: 0 2px 4px rgba(0, 0, 0, 0.6);
}
</style>
