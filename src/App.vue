<template>
  <div id="app">
    <h1>{{ counter }}</h1>
    <p>
      {{ getMessage() }}
    </p>
    <button @click="counter++">Increase</button> | <button @click="counter--">Decrease</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      counter:  0,
    }
  },
  methods: {
    getMessage() {
      return (this.counter < 5) ? "Меньше 5" : "Больше либо равно 5";
    },
  },
}
</script>
