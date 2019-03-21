<template>
  <div>
    <v-toolbar color="teal">
      <v-toolbar-side-icon></v-toolbar-side-icon>
      <v-toolbar-title>Title</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn v-for="item in items" :key="item" flat>
          <v-icon size="24px">{{ item.icon }}</v-icon> {{ item.title }}
        </v-btn>
      </v-toolbar-items>
    </v-toolbar>
  </div>
</template>

<script>
export default {
  name: 'LayoutHeader',
  data() {
    return {
      items: [
        {
          icon: 'hpme',
          title: 'Home',
          to: '/'
        },
        {
          icon: 'info',
          title: 'About',
          to: '/about'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'FunxtionID'
    }
  }
}
</script>

<style scoped></style>
