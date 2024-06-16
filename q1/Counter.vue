<template>
    <div>
        <h1>Counter: {{ counter }}</h1>
        <button @click="increment">Increment</button>
        <button @click="decrement">Decrement</button>
        <button @click="reset">Reset</button>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

// Define a reactive variable for the count
const counter = ref(0);

// Implement methods to increment, decrement, and reset the count
const increment = () => {
    counter.value++;
};

const decrement = () => {
    counter.value--;
};

const reset = () => {
    counter.value = 0;
};
</script>
