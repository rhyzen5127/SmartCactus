<template>
    <div>
        <v-dialog v-model="cactusDialog">
        </v-dialog>
    </div>
</template>


<script>

export default {
  props: {
    cactusDialog: {
      type: Boolean,
      require: false,
      default: false,
    },
  },

  components: {
  },

  data: () => ({
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