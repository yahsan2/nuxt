<template>
  <div class="page page--home">
    <a href="https://nuxtjs.org/" target="_blank">
      <nuxt-logo />
    </a>
    <div class="plus">+</div>
    <a href="https://vuetifyjs.com" target="_blank">
      <vuetify-logo />
    </a>
  </div>
</template>

<script>
  import NuxtLogo from '~components/NuxtLogo.vue'
  import VuetifyLogo from '~components/VuetifyLogo.vue'

  export default {
    components: {
      NuxtLogo,
      VuetifyLogo
    }
  }
</script>

<style>
  .plus {
    font-size: 80px;
    margin: 0 60px;
  }
</style>
