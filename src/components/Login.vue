<template>
  <v-container>
    <v-card>
      <v-img
        max-height="300"
        justify-center
        src="https://vbis.vbeyond.co.th/uploads/vbe.png"
      ></v-img>
      <v-card-title class="text-center">
        <h2>VBIS System</h2>
      </v-card-title>
      <v-card-text>
        <v-form @submit.prevent="login">
          <v-text-field
            clearable
            label="Code"
            variant="outlined"
            v-model="username"
            required
          ></v-text-field>
          <v-text-field
            clearable
            label="Password"
            variant="outlined"
            v-model="password"
            type="password"
            required
          ></v-text-field>
          <v-btn color="primary" type="submit" block class="mb-2">Login</v-btn>
          <v-btn color="dark" type="submit" block
            >Login With Microsoft</v-btn
          >
        </v-form>
      </v-card-text>
    </v-card>
  </v-container>
</template>

<script>
export default {
  name: "LoginPage",
  data() {
    return {
      username: "",
      password: "",
    };
  },
  methods: {
    login() {
      // You can implement your login logic here
      console.log("Logging in...");
    },
  },
};
</script>
