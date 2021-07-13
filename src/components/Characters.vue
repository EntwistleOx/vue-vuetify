<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <v-img
          :src="require('../assets/logo.svg')"
          class="my-3"
          contain
          height="80"
        />
      </v-col>

      <v-col cols="12">
        <v-row justify="center">
          <v-card
            v-for="(character, i) in characters"
            :key="i"
            class="subheading mx-3 mb-6"
            target="_blank"
          >
            <v-img
              class="white--text align-end"
              height="200px"
              :src="character.imgUrl"
            >
            </v-img>
            <v-card-title>{{ character.name }}</v-card-title>
          </v-card>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import { characters } from "../data/index";

export default {
  name: "Characters",

  data: () => ({
    characters: characters,
  }),
};
</script>
