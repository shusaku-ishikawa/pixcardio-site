<template>
  <v-app>
    <v-app-bar
      fixed
      app
      color="white"
    >
      <v-toolbar-title>
        <PixcardioLogo />
      </v-toolbar-title>
      <v-spacer />
      <v-btn
        icon
        @click.stop="rightDrawer = !rightDrawer"
      >
        <v-icon>menu</v-icon>
      </v-btn>
    </v-app-bar>
    <v-main>
      <nuxt />
    </v-main>
    <v-navigation-drawer
      v-model="rightDrawer"
      :right="right"
      temporary
      fixed
    >
      <v-list>
        <v-list-item @click.native="right = !right">
          <v-list-item-action>
            <v-icon light>
              repeat
            </v-icon>
          </v-list-item-action>
        </v-list-item>
        <v-list-item>
          <v-list-content>
            <a href="/">Top</a>
          </v-list-content>
        </v-list-item>
        <v-list-item>
          <v-list-content>
            <a href="/terms">Terms Of Service</a>
          </v-list-content>
        </v-list-item>
        <v-list-item>
          <v-list-content>
            <a href="/privacy_policy">Privacy Policy</a>
          </v-list-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-footer
      app
      class="grey--text text-darken-2"
    >
      <div class="text-caption text-sm-body-2 text-md-body-2 text-center">
        <span>&copy; {{ new Date().getFullYear() }} PIXCARDIO LLC All Rights Reserved.</span>
      </div>

    </v-footer>
  </v-app>
</template>

<script>
import PixcardioLogo from '@/components/PixcardioLogo'

export default {
  components: {
    PixcardioLogo,
  },
  data () {
    return {
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>
