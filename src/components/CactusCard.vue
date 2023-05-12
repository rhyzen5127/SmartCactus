<template v-slot:default="{ item }">
  <v-card class="ma-5" height="256">

    <!-- Full Information Card Pop up. -->
    <div>
      <v-dialog v-model="cactusDialog">
        <v-card class="ma-5" height="800"></v-card>
      </v-dialog>
    </div>

    <!-- Card -->
    <v-row>
      <v-col md="3">
        <!-- pic -->
      </v-col>
      <v-col md="7">
        <v-card-title>{{ name }}</v-card-title>
        <v-card-text>{{ detail }}</v-card-text>
      </v-col>
      <v-col md="2">
        <v-btn height="256" width="150" color="green" @click="cactusDialog = true">
        </v-btn>
      </v-col>
    </v-row>


    <!-- 
  อันที่ดูค่ามี
    -ความชื้น
    -อุณหภูมิ 
    -ความเข้มแสง
    -ความชื้นในดิน

  อันที่ user ควบคุมได้
    -รดน้ำ (switch)
    -เปิดปิดหลังคากันแสง (switch)
  -->

  </v-card>
</template>

  
<script>

export default {
  props: {
    name: {
      type: String,
      require: false,
      default: "n u l l",
    },
    detail: {
      type: String,
      require: false,
      default: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
    },
  },

  components: {
  },

  data: () => ({
    logoPath: new URL("@/Images/Logo.png", import.meta.url).href,
    cactusLogoPath: new URL("@/Images/CactusLogo.png", import.meta.url).href,
    cactusDialog: false,
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