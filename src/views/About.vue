<template>
  <div class="content__page">
    <div class="content__page-main custom-layout">
      <h1>{{content.menu.about}}</h1>
      <div v-html="content.about.content"/>
    </div>
    <Footer :content="content"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Footer from "@/components/Footer.vue";

export default {
  name: "about",
  props: {
    content: Object
  },
  components: { Footer }
};
</script>
