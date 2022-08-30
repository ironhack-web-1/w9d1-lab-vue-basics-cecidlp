<template>
  <div>
    <NavBar />
    <FooterPage />
  </div>
    <div>
    <p>¿Cuánto es 2 + 9?</p>
     <label>
    <input type="radio" value="5" v-model="MathOperation"/>
    5
  </label>
  <label>
    <input type="radio" value="9" v-model="MathOperation"/>
    9
  </label>
  <label>
    <input type="radio" value="11" v-model="MathOperation"/>
    11
  </label>
  <div v-if="MathOperation === '11'">Muy bien! Has resuelto la suma</div>
  <div v-else> Ups, no </div>
  </div>
  <IteracionCuatro />
</template>

<script>
import FooterPage from "./components/FooterPage.vue";
import NavBar from "./components/NavBar.vue";
import IteracionCuatro from "./components/IteracionCuatro.vue";
export default {
  components: {
    NavBar,
    FooterPage,
    IteracionCuatro,
},
  data() {
      return {
        MathOperation: 2 + 9,
      };
    },
};
</script>

<style></style>
