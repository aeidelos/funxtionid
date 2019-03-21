<template>
  <v-app dark>
    <Header />
    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>
    <Footer />
  </v-app>
</template>

<script>
import Header from '@/components/layout/header/Header'
import Footer from '@/components/layout/footer/Footer'
export default {
  components: {
    Header,
    Footer
  },
  data() {
    return {}
  }
}
</script>
