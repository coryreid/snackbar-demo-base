<template>
  <v-app>

    <v-toolbar fixed app>
      <v-toolbar-title>Snackbar Demo</v-toolbar-title>
    </v-toolbar>

    <v-content>
      <v-container fluid>
        <v-slide-y-transition mode="out-in">
          <v-layout column align-center>
			<snackbar-store/>
            <router-view></router-view>

          </v-layout>
        </v-slide-y-transition>
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
import snackbarStore from '@/components/SnackbarStore'

export default {
  data() {
    return {}
  },
  components: {
    snackbarStore
  }
}
</script>
