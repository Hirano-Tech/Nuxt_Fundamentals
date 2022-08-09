<template>
  <section class='container'>
    <div>
      <logo />
      <h1 class='title'>nuxt-fundamentals</h1>
      <h2 class='subtitle'>My gnarly Nuxt.js project</h2>

      <div class='links'>
        <nuxt-link v-for='post in posts' :to="{name: 'posts-id', params: {id: post.id}}" :key='post.id' class='button--grey'>{{ post.title }}</nuxt-link>
      </div>
    </div>
  </section>
</template>

<script>
  import Logo from '~/components/Logo.vue'

  export default {
    components: {
      Logo
    },

    computed: {
      posts() {
        return this.$store.state.posts.all
      }
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