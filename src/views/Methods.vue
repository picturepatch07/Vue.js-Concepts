<template>
    <div>
        <button @click="sayHello()">Click Me</button>
        <h1>You pressed button {{ counter }} times</h1>
    </div>
</template>

<script>

export default {
    data() {
        return {
            counter: 0
        }
    },
    methods: {
        sayHello() {
            this.counter++;
            console.log("Hello");
        }
    },
}
</script>

<style lang="scss" scoped>

</style>