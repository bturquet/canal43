<template>
  <v-app dark>
    <v-navigation-drawer
      :mini-variant.sync="miniVariant"
      :clipped="clipped"
      v-model="drawer"
      fixed
      app
    >
      <v-list>
        <v-list-tile
          router
          :to="item.to"
          :key="i"
          v-for="(item, i) in items"
          exact
        >
          <v-list-tile-action>
            <v-icon v-html="item.icon"></v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title v-text="item.title"></v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
    <v-toolbar fixed app :clipped-left="clipped">
      <v-toolbar-side-icon @click="drawer = !drawer"></v-toolbar-side-icon>
      <v-btn
        icon
        @click.stop="miniVariant = !miniVariant"
      >
        <v-icon v-html="miniVariant ? 'chevron_right' : 'chevron_left'"></v-icon>
      </v-btn>
      <v-btn
        icon
        @click.stop="clipped = !clipped"
      >
        <v-icon>web</v-icon>
      </v-btn>
      <v-toolbar-title v-text="title"></v-toolbar-title>
      <v-spacer></v-spacer>
    </v-toolbar>
    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>
    <v-footer :fixed="fixed" app>
      <span>&copy; 2018 CANAL43</span> - <v-icon>fa-facebook-square</v-icon> - <v-icon>fa-twitter-square</v-icon> - <v-icon>fa-instagram</v-icon>
    </v-footer>
  </v-app>
</template>

<script>
  export default {
    data () {
      return {
        clipped: false,
        drawer: true,
        fixed: false,
        items: [
          { icon: 'apps', title: 'Welcome', to: '/' },
          { icon: 'calendar_today', title: 'Calendrier', to: '/calendrier' },
          { icon: 'view_list', title: 'Programmation', to: '/programmation' },
          { icon: 'info', title: 'Infos Pratiques', to: '/infos' },
          { icon: 'receipt', title: 'Billetterie', to: '/billetterie' },
          { icon: 'group', title: 'Partenaires', to: '/partenaires' },
          { icon: 'contact_phone', title: 'Contact', to: '/contact' }
        ],
        miniVariant: false,
        right: true,
        rightDrawer: false,
        title: 'canal43'
      }
    }
  }
</script>
