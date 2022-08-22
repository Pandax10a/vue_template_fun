<template>
    <div>
        <h1>{{blog_title}}</h1><br>
        <h3>{{blog_content}}</h3><br>
        <img :src ="blog_image_url">
    </div>
</template>

<script>


    export default {
          data() {
    return {
      blog_content: `this is the quality blog content`,
      blog_title: `Read this please`,
      blog_image_url: `https://projectpokemon.org/images/shiny-sprite/gyarados-mega.gif`
    }
  },
      name: 'template-fun'
    }
</script>

<style scoped>

</style>