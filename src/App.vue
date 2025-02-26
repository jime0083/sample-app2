<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <v-app-bar-nav-icon></v-app-bar-nav-icon>
      <div class="d-flex align-center">
        <span>マイアドレス帳</span>
      </div>
      <v-spacer></v-spacer>
    </v-app-bar>
    <SideNav></SideNav>
    <v-main>
      
    </v-main>
  </v-app>
</template>

<script>
import SideNav from './components/SideNav.vue';


export default {
  name: 'App',

  components: {
    SideNav
  },

  data: () => ({
    //
  }),
};
</script>
