<template>
  <div class="sign-in">
    <div class="form-container">
      <label class="flex-child">
        <input v-model="userName" placeholder="User Name">
      </label>
      <label class="flex-child">
        <input v-model="password" placeholder="Password">
      </label>
      <label class="flex-child">
        <button >Sign In</button>
      </label>
      <NuxtLink to="/sign-up">Sign Up</NuxtLink>
    </div>
  </div>
</template>
<style lang="scss">
@import '../assets/styles/sign-in';
</style>
<script>
import axios from "axios";

export default {
  props: [],
  data() {
    return {
      userName: null,
      password: null
    };
  },
  methods: {
    handleInput() {
      this.$emit('input', this.value);
    },
  }
}
</script>

