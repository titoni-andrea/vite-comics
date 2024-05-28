<script >
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
components: {
  AppHeader,
  AppMain,
  AppFooter,
},

  data() {
    return {
      prova: "ciao",
    }
  },

  methods: {
    ciao() {
      console.log(this.prova);
    }
  },

  mounted() {
    this.ciao();
  },
}

</script>

<template>

  <AppHeader/>
  <AppMain/>
  <AppFooter/>

</template>

<style scoped>

</style>
