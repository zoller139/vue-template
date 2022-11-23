<script setup>
import { reactive, ref } from 'vue'
import { useMouse } from './components/bar'
const dd = reactive({ cs: 1 })
const id = ref(0)
console.log(1111)
const { x, y } = useMouse()
function hddd() {
  console.log(dd)
  console.log(id)
}
</script>

<template>
  <div>
    {{dd.cs}}
    <button @click="dd.cs++">add</button>
    <button @click="hddd">add</button>
    <p>{{y}} {{x}}</p>
  </div>
</template>

<style scoped>

</style>
