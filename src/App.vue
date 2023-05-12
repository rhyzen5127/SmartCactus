<template>
  <v-app style="background-color: #AFA77B;">
    <v-main>
      <NavBar />
      <router-view :key="$route.path" />
    </v-main>
  </v-app>
</template>

<script>
// Components
import { RouterLink, RouterView } from 'vue-router'
import NavBar from '@/components/NavBar.vue'

export default {
  name: 'App',

  components: {
    NavBar,
  },

  data: () => ({
  }),

}
</script>