<script setup>
  import { ref } from 'vue'



  const eggs = ref(0)
  const milk = ref(0)
  const beef = ref(0)



  function incrementEggs() {
    eggs.value++
  }
  function incrementMilk() {
    milk.value++
  }
  function incrementBeef() {
    beef.value++
  }
  function decrementEggs() {
    if (eggs.value > 0) eggs.value--
  }
  function decrementMilk() {
    if (milk.value > 0) milk.value--
  }
  function decrementBeef() {
    if (beef.value > 0) beef.value--
  }




</script>


<template>
  <div>
    Eggs: <button @click="incrementEggs"> + </button>
    {{eggs}} <button @click="decrementEggs"> - </button>
  </div>
  <div></div>
  <div>
    Milk : <button @click="incrementMilk"> + </button>
    {{milk}} <button @click="decrementMilk"> - </button>
  </div>
  <div></div>
  <div>
    Beef : <button @click="incrementBeef"> + </button>
    {{beef}} <button @click="decrementBeef"> - </button>
  </div>


</template>


