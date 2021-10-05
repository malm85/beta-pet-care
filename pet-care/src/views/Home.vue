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

      <v-toolbar-title>PetCare</v-toolbar-title>
    </v-app-bar>

    <v-main>
        
            <Card />
      
      <Example/>
    </v-main>
  </v-app>
</template>

<script>
  import Card from '../components/Card.vue'
  import Example from '../components/Example.vue'

  export default {
    data: () => ({ drawer: null }),
    
    name: 'Home',

    components: {
      Card,
      Example,
    }
  }
</script>
