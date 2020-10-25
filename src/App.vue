<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <div class="d-flex align-center">
        <v-img
          alt="SimpleApps Logo"
          class="shrink mr-2"
          contain
          :src="require('./assets/logo.svg')"
          transition="scale-transition"
          width="40"
        />
        
        <h2>Simple Apps</h2>
      </div>
      
      <v-spacer></v-spacer>
      
      <span>
        <span class="mr-2">Version 0.1.0 Beta</span>
        <v-icon>code</v-icon>
      </span>
    </v-app-bar>
    <v-main></v-main>
    <BottomNav />
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue'
import TopToolbar from '@/components/TopToolbar.vue'
import BottomNav from '@/components/BottomNav.vue'

export default Vue.extend({
  name: 'App',
  components: {
    BottomNav,
    TopToolbar
  },
  
  data: () => ({
    //
  })
})
</script>

<style lang="scss">
#app {
  background-color: #7d121f;
}
</style>
