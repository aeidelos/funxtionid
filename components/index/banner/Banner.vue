<template>
  <section>
    <v-parallax :src="hero" height="600" alt="funxtion image">
      <v-layout column align-center justify-center class="white--text">
        <img src="assets/vuetify.png" alt="Vuetify.js" height="200" />
        <h1 class="white--text mb-2 display-1 text-xs-center">
          Parallax Template
        </h1>
        <div class="subheading mb-3 text-xs-center">Powered by Vuetify</div>
        <v-btn class="blue lighten-2 mt-5" dark large href="/pre-made-themes">
          Get Started
        </v-btn>
      </v-layout>
    </v-parallax>
  </section>
</template>

<script>
import Hero from '@/assets/img/hero.jpeg'
export default {
  name: 'IndexBanner',
  data() {
    return {
      hero: Hero
    }
  }
}
</script>

<style scoped></style>
