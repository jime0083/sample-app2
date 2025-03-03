<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <v-app-bar-nav-icon @click="toggleSideMenu"></v-app-bar-nav-icon>
      <div class="d-flex align-center">
        <span>マイアドレス帳</span>
      </div>
      <v-spacer></v-spacer>
    </v-app-bar>
    <SideNav />

    <v-content>
      <router-view />
    </v-content>
  </v-app>
</template>

<script>
import { mapActions } from 'vuex';
import SideNav from './components/SideNav.vue';


export default {
  name: 'App',

  components: {
    SideNav
  },

  data: () => ({
    //
  }),
  methods:{
      ...mapActions(['toggleSideMenu'])
  }
};
</script>
