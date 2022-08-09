<template>
  <div class='container'>
    <TheNavbar />
    <nuxt />
  </div>
</template>

<script>
  import TheNavbar from '@/components/TheNavbar'

  export default {
    components: {
      TheNavbar
    }
  }
</script>

<style>
  .button--green {
    color: #3b8070;
    text-decoration: none;
    border: 1px solid #3b8070;
    border-radius: 4px;
    padding: 10px 30px;
    display: inline-block;
  }

  .button--green:hover {
    background-color: #3b8070;
    color: #fff;
  }

  .button--grey {
    color: #35495e;
    text-decoration: none;
    border: 1px solid #35495e;
    border-radius: 4px;
    padding: 10px 30px;
    margin-left: 15px;
    display: inline-block;
  }

  .button--grey:hover {
    background-color: #35495e;
    color: #fff;
  }
</style>