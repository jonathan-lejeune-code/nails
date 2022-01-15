<template>
  <v-app dark>
    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      temporary
      app
      color="pink lighten-3"
    >
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon class="white--text">{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title class="white--text" v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar color="pink lighten-3" :clipped-left="clipped" fixed app>
      <v-app-bar-nav-icon class="white--text" @click.stop="drawer = !drawer" />
      <router-link to="/" style="text-decoration: none">
        <v-toolbar-title class="white--text" v-text="title" />
        <v-spacer />
      </router-link>
    </v-app-bar>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>

    <v-footer class="justify-center" :absolute="!fixed" app>
      <span>&copy; {{ new Date().getFullYear() }} - Nails ART </span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Accueil',
          to: '/',
        },
        {
          icon: 'mdi-home-circle',
          title: 'Présentation',
          to: '/about',
        },
        {
          icon: 'mdi-currency-eur',
          title: 'Tarifs',
          to: '/tarif',
        },

        {
          icon: 'mdi-picture-in-picture-top-right',
          title: 'Photos',
          to: '/photos',
        },
        {
          icon: 'mdi-phone-classic',
          title: 'Contact',
          to: '/contact',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'LOGO Nails ART',
    }
  },
}
</script>
