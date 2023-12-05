<template>
  <v-app>
    <v-main>
      <LoginPage/>
    </v-main>
  </v-app>
</template>

<script>
import LoginPage from './components/Login.vue'

export default {
  name: 'App',

  components: {
    LoginPage,
  },

  data: () => ({
    //
  }),
}
</script>
