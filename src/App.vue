<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <v-toolbar-title>Julia Con 2021</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn>Home</v-btn>
      <v-btn>Login</v-btn>
    </v-app-bar>

    <v-content>
      <router-view />
    </v-content>
  </v-app>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'App',

  data() {
    return {
      //
    }
  }
})
</script>
