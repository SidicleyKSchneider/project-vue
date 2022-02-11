<template>
  <v-coontainer fluid>
    <v-row justify="center">
      <v-col cols="12" md="4" lg="3" class="text-center">
        <h6 class="headline">Login</h6>
        <v-text-field v-model="token" label="Token"></v-text-field>
        <v-btn depressed dark block color="green" @click="login"> Login </v-btn>
        <v-btn text block @click="loginAsGuest"> entrar como visitante </v-btn>
      </v-col>
    </v-row>
  </v-coontainer>
</template>

<script>
export default {
  name: "LoginPage",
  data() {
    return {
        token:"",
    };
  },
  methods: {
    login() {
        alert({this.token})
    },
    loginAsGuest() {
        //TODO
    },
  },
};
</script>

<style scoped>
</style>