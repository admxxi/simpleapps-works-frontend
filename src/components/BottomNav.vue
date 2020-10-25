<template>
  <v-bottom-navigation app fixed grow v-model="activeItem" color="primary"> </v-bottom-navigation>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

@Component
export default class BottomNav extends Vue {
  activeItem: string = 'top'
}
</script>
