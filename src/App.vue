<script setup>
import {ref} from "vue"

let count = ref(0)

const addToCount = () => {
  count.value++
}

const subtractFromCount = () => {
  count.value--
}
</script>

<template>
  <main>
    <div>
      <h4>The current count is ...</h4>
      <h1>
        {{ count }}
      </h1>
      <button @click="subtractFromCount">-</button>
      <button @click="addToCount">+</button>
    </div>
  </main>
</template>

<style scoped lang="sass">
main
  background-color: aliceblue
  width: 100vw
  height: 100vh
  display: flex
  justify-content: center
  align-items: center

  div
    color: #000
    text-align: center

</style>