<template>
  <div>
    <NavBar />
    <br>
    <FooterPage />
  </div>
  <br>
  <IteracionTres />
  <br>
  <br>
  <IteracionCuatro />
</template>

<script>
import FooterPage from "./components/FooterPage.vue";
import NavBar from "./components/NavBar.vue";
import IteracionTres from "./components/IteracionTres.vue";
import IteracionCuatro from "./components/IteracionCuatro.vue";
export default {
  components: {
    NavBar,
    FooterPage,
    IteracionTres,
    IteracionCuatro,
  },
};
</script>

<style></style>
