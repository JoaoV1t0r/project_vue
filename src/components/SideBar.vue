<template>
  <div class="ma-12 pa-12">
    <v-card>
      <v-navigation-drawer
        permanent
        expand-on-hover
      >
        <v-list>
          <v-list-item class="px-2">
            <v-list-item-avatar>
              <v-img src="https://randomuser.me/api/portraits/women/85.jpg"></v-img>
            </v-list-item-avatar>
          </v-list-item>

          <v-list-item link>
            <v-list-item-content>
              <v-list-item-title class="text-h6">
                Sandra Adams
              </v-list-item-title>
              <v-list-item-subtitle>sandra_a88@gmail.com</v-list-item-subtitle>
            </v-list-item-content>
          </v-list-item>
        </v-list>

        <v-divider></v-divider>

        <v-list
          nav
          dense
        >
          <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-folder</v-icon>
            </v-list-item-icon>
            <v-list-item-title>My Files</v-list-item-title>
          </v-list-item>
          <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-account-multiple</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Shared with me</v-list-item-title>
          </v-list-item>
          <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-star</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Starred</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-navigation-drawer>
    </v-card>
  </div>
</template>

<script>
import  Vue  from 'vue';
export default Vue.extend({
  name:"SideBar",
  data() {
    return {
      drawer: true,
      user: {
        name: "João Vitor",
        photo:
          "https://avatars.githubusercontent.com/u/76921187?s=400&u=7e56b6f8d503cd4dcf464016b9a7aa3750239456&v=4",
      },
      items: [
        {
          title: "Home",
          icon: "mdi-home-city",
          url: "/",
        },
        {
          title: "Minha conta",
          icon: "mdi-account",
          url: "/my-account",
        },
        {
          title: "Clientes",
          icon: "mdi-account-group-outline",
          url: "/about",
        },
      ],
      mini: true,
    };
  },
  methods: {
    redirect(url) {
      this.$router.replace(url);
    },
  },
});
</script>