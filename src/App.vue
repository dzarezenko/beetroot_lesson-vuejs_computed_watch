<template>
  <div id="app">
    <h1>{{ counter }}</h1>
    <p>
      {{ getMessage() }}
    </p>
    <p>
      {{ counter2 }}
    </p>
    <button @click="counter++">Increase</button> | <button @click="counter--">Decrease</button>
    <br />
    <button @click="counter2++">Increase 2</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      counter: 0,
      counter2: 0,
    }
  },
  methods: {
    getMessage() {
      console.log("Method called");
      return (this.counter < 5) ? "Меньше 5" : "Больше либо равно 5";
    },
  },
}
</script>
