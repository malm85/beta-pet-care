<template>
  <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      app
    >
      <!--  -->
    </v-navigation-drawer>
    <v-app-bar color="green" prominent app>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>PetCare</v-toolbar-title>
      
    </v-app-bar>

    <v-main>
      <table>
        <th><Card /></th>
        <th><Calendar/></th>
      </table>
      <div>
        <p>Nuestros servicios estan pensados para el cuidado de su mascota</p>
      </div>
      <div> 
        <Example/>
      </div>
    </v-main>
  </v-app>
</template>

<script>
  import Card from '../components/Card.vue'
  import Example from '../components/Example.vue'
  import Calendar from '../components/Calendar.vue'

  export default {
    data: () => ({ drawer: null }),
    
    name: 'Home',

    components: {
      Card,
      Example,
      Calendar,
    }
  }
</script>
