<template>
  <v-app>
    <v-app-bar app color="deep-purple" dark>
      <v-app-bar-nav-icon></v-app-bar-nav-icon>
      <v-toolbar-title>Vue con Vuetify</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <Characters />
    </v-main>
  </v-app>
</template>

<script>
import Characters from "./components/Characters.vue";

export default {
  name: "App",

  components: {
    Characters,
  },

  data: () => ({
    //
  }),
};
</script>
