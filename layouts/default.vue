<template>
  <v-app light>
    <v-toolbar fixed app :clipped-left="clipped"  >
      <v-toolbar-title v-text="title"></v-toolbar-title>
      <v-spacer></v-spacer>
    </v-toolbar>
    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
import 'vuetify/dist/vuetify.min.css'
  export default {
    data () {
      return {
        clipped: false,
        fixed: false,
        miniVariant: false,
        right: true,
        title: 'KANBAN'
      }
    }
  }
</script>
