<template>
  <v-app>
    <v-app-bar app color="light-green lighten-2">
      <router-link style="text-decoration: none; color: inherit" to="/">
        <v-app-bar-title>
          <h4 class="white--text">Test</h4>
        </v-app-bar-title>
      </router-link>
      <v-spacer></v-spacer>
      <router-link style="text-decoration: none; color: inherit" to="/form">
        <v-btn icon>
          <v-icon>mdi-message-text</v-icon>
        </v-btn>
      </router-link>
    </v-app-bar>
    <v-main> <router-view /> </v-main>
  </v-app>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "App",

  data: () => ({
    //
  }),
});
</script>
