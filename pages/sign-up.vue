<template>
  <div class="sign-up-form">
    <input v-model="username" placeholder="Username">
    <input v-model="passwordOne" placeholder="Password">
    <input v-model="passwordTwo" placeholder="Repeat Password">
    <input v-model="email" placeholder="E-mail">
  </div>
</template>


<script>
import axios from 'axios';

export default {
  data() {
    return {
      username: null,
      passwordOne: null,
      passwordTwo: null,
      email: null
    };
  }
}
</script>
