<template>
  <div class="mathOperation">
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
  <div class="correct" v-if="MathOperation === '11'">Muy bien! Has resuelto la suma</div>
  <div class="incorrect" v-else> Ups, no </div>
  </div>
</template>

<script>
export default {
    data() {
      return {
        MathOperation: 2 + 9,
      };
    },
}
</script>

<style>
    .mathOperation {
        font-family: Raleway;
    }
    .mathOperation p {
        font-size: 1.2em;
        color: #EC729B;
    }
    .incorrect {
        color: #a62121;
    }
</style>