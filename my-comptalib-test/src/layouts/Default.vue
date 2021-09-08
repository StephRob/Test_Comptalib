<template>
  <div>
    <Header />
    <slot/>
    <Footer />
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
import Header from "./Header.vue";
import Footer from "./Footer.vue";

export default {
  components: {
    Header,
    Footer,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@100;400;700&display=swap");
body,
button,
input,
optgroup,
select,
textarea {
  font-family: "Roboto", sans-serif !important;
  margin: 0;
  padding: 0;
  line-height: 1.5;
}
</style>
