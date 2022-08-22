<template>
    <div>
        <section v-if = "show_post">
            <article v-for="(user, index) in content_users" :key="index">
                <h1>{{content_users[index][`blog_title`]}}</h1><br>
                <h3>{{content_users[index][`blog_content`]}}</h3><br>
                <img :src = "content_users[index][`blog_image_url`]">
                <!-- <h3>{{blog_content}}</h3><br> -->
                <!-- <img :src ="blog_image_url"><br> -->
            </article>
            
        </section>
        <button @click="change_button()">Change</button>
    </div>
</template>

<script>


    export default {
          data() {
    return {
        content_users:[{
      blog_content: `this is the quality blog content 1`,
      blog_title: `Read this please 1`,
      blog_image_url: `https://projectpokemon.org/images/shiny-sprite/gyarados-mega.gif`,
      show_post: true,
    },
    {
      blog_content: `this is the quality blog content 2`,
      blog_title: `Read this please 2`,
      blog_image_url: `https://projectpokemon.org/images/shiny-sprite/magikarp-f.gif`,
      show_post: true,
    },
    {
      blog_content: `this is the quality blog content 3`,
      blog_title: `Read this please 3`,
      blog_image_url: `https://projectpokemon.org/images/shiny-sprite/omastar.gif`,
      show_post: true,
    }],
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