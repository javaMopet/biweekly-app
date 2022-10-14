<template>
  <div class="login__container">
    <ul class="login__navigation">
      <li class="login__navigation--item active"><a href="#">Entrar</a></li>
      <li class="login__navigation--item"><a href="#">Registrarse</a></li>
    </ul>
    <form action="submit" class="login__form">
      <q-input
        v-model="email"
        color="indigo-3"
        input-style="color:white"
        label-color="indigo-3"
        label="Email"
        type="text"
      />
      <q-input
        v-model="password"
        color="indigo-3"
        input-style="color:white"
        label-color="indigo-3"
        label="Password"
        type="password"
      />
      <!-- <label for="login-sign-up" class="login__label--checkbox">
			<input id="login-sign-up" type="checkbox" class="login__input--checkbox" />
			Keep me Signed in
		</label> -->
      <button class="login__submit" @submit="submit">Entrar</button>
    </form>
    <a href="#" class="login__forgot">¿Olvidaste tu Contraseña?</a>
  </div>
</template>
<script setup>
import { ref } from "vue";

const email = ref("");
const password = ref("");

const submit = () => {
  alert("working!");
};
</script>

<style scoped lang="scss" src="../assets/scss/login_main.scss" />
