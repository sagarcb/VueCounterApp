<script setup>
import { ref } from "vue"
const count = ref(0);

console.log(count);

const addToCount = () => {
  count.value++;
}

const subtractFromCount = () => {
  count.value--;
}
</script>

<!--<script>-->
<!--export default({-->
<!--  data() {-->
<!--    return {-->
<!--      count: 0-->
<!--    }-->
<!--  },-->
<!--  methods: {-->
<!--    addToCount(){-->
<!--      this.count = this.count + 1;-->
<!--    },-->
<!--    subtractFromCount() {-->
<!--      this.count = this.count - 1;-->
<!--    }-->
<!--  }-->
<!--})-->
<!--</script>-->

<template>
  <main>
    <div>
      <h4>The current count is...</h4>
      <h1>{{count}}</h1>
      <button @click="subtractFromCount()">-</button>
      <button @click="addToCount()">+</button>
    </div>
  </main>
</template>

<style scoped>
main {
  background-color: aliceblue;
  width: 100vw;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}
div {
  text-align: center;
}
</style>