<template>
    <div>
        <section v-if = "show_post">
            <h1>{{blog_title}}</h1><br>
            <h3>{{blog_content}}</h3><br>
            <img :src ="blog_image_url"><br>
            
        </section>
        <button @click="change_button()">Change</button>
    </div>
</template>

<script>


    export default {

          data() {
    return {
      blog_content: `this is the quality blog content`,
      blog_title: `Read this please`,
      blog_image_url: `https://projectpokemon.org/images/shiny-sprite/gyarados-mega.gif`,
      show_post: true,
    }
  },        
  methods: {
            change_button() {
                if(this.show_post){
                    this.show_post = false;
                } else if (this.show_post === false) {
                    this.show_post = true;
                }
            }
        },
      name: 'template-fun'
    }
</script>

<style scoped>

</style>