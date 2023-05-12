<template>
  <div>
    <v-app-bar color="#2B4D1B" prominent>
      <v-toolbar-title>
        <v-row>
          <v-col md="1"><v-img :src="cactusLogoPath" max-height="48" /></v-col>
          <v-col md="11"><v-img :src="logoPath" max-width="200" max-height="48" /></v-col>
        </v-row>
      </v-toolbar-title>
      <v-spacer>
      </v-spacer>
    </v-app-bar>
  </div>
</template>

  
<script>

export default {
  props: {
    loggedIn: {
      type: Boolean,
      require: true,
      default: false,
    },
    name: {
      type: String,
      require: true,
      default: "Rhyzen",
    },
  },

  components: {
  },

  data: () => ({
    logoPath: new URL("@/Images/Logo.png", import.meta.url).href,
    cactusLogoPath: new URL("@/Images/CactusLogo.png", import.meta.url).href,
  }),

  methods: {
  }

}
</script>
  
<style scoped>
/* .hover-logo {
    cursor: pointer;
  } */
</style>