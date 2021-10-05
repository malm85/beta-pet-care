<template>
  <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      app
    >
      <!--  -->
    </v-navigation-drawer>

    <v-app-bar app>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>Application</v-toolbar-title>
    </v-app-bar>

    <v-main>
      <Calendar/>
    </v-main>
  </v-app>
</template>

<script>
  import Calendar from '../components/Calendar'

  export default {
    data: () => ({ drawer: null }),
    
    name: 'Home',

    components: {
      Calendar,
    },
  }
</script>
