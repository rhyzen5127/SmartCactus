<script setup>

</script>

<template>
  <div class="pa-12 d-flex align-center justify-center">
    <v-card height="760" width="1200">
      <div>
        <v-virtual-scroll :height="600" class="ma-16" :items="cactuses">
          <CactusCard :name='cactuses.name'/>
        </v-virtual-scroll>

      </div>
    </v-card>
  </div>
</template>


  
<script>
import CactusCard from '@/components/CactusCard.vue'

export default {
  props: {
  },

  components: {
    CactusCard,
  },

  data: () => ({
    cactuses: [
      { id: 0, name: 'Item 0', description: 'ต้นที่ 1.' },
      { id: 1, name: 'Item 1', description: 'ต้นที่ 2.' },
      { id: 2, name: 'Item 2', description: 'ต้นที่ 3.' },
    ],
  }),

  methods: {
  }

}
</script>

<style></style>