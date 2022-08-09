<template>
  <section class='container'>
    <div>
      <logo />
      <h1 class='title'>nuxt-fundamentals</h1>
      <h2 class='subtitle'>My gnarly Nuxt.js project</h2>

      <div class='links'>
        <a href='https://nuxtjs.org' target='_blank' class='button--green'>Documentation</a>
        <a href='https://github.com/nuxt/nuxt.js' target='_blank' class='button--grey'>GitHub</a>
      </div>
    </div>
  </section>
</template>

<script>
  import Logo from '~/components/Logo.vue'

  export default {
    components: {
      Logo
    }
  }
</script>

<style scoped>
  .container {
    text-align: center;
    display: flex;
      justify-content: center;
      align-items: center;
  }

  .title {
    font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    font-size: 100px;
    font-weight: 300;
    letter-spacing: 1px;
    display: block;
  }

  .subtitle {
    color: #526488;
    font-size: 42px;
    font-weight: 300;
    word-spacing: 5px;
  }

  .links { padding-top: 15px; }
</style>