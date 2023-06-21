<!-- javascript code -->
<script>
export default {
    data: () => ({
        counter: 0,
    }),
    methods: {
        increment() {
            this.counter++;
        },
        decrease() {
            this.counter--;
        },
        reset() {
            this.counter = 0;
        },
    },
};
</script>
<!-- end javascript code -->

<template>
    <div class="container">
        <h1>Brayan Córdova - Web Developer</h1>
        <hr />
        <img src="./assets/logo.svg" alt="logo vue" width="125" height="125" />
        <small>
            <h1 class="name">Hello World from Vue.js 3</h1>
        </small>
        <hr />

        <h2>Counter: {{ counter }}</h2>
        <button @click="increment()">+1</button>
        <button @click="decrease()">-1</button>
        <button @click="reset()">Reset</button>
    </div>
</template>

<style scoped>
.container {
    text-align: center;
    background-color: #ccc;
}

small {
    color: #666;
}

h1 {
    font-weight: bolder;
}

h2 {
    font-size: 2.5rem;
}

button {
    cursor: pointer;
    font-size: 1.5rem;
    margin: 0px 6px;
}
</style>
