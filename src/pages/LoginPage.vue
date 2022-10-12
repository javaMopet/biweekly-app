<template>
  <div class="login">Mi login</div>
  <q-btn color="primary" icon="check" label="OK" @click.prevent="submit" />
</template>
<script setup>

const submit = ()=> {
  alert("working!");
}
</script>

<style scoped lang="scss" src="../assets/scss/login_main.scss" />
