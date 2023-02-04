<template>
    <div class="home">
        <!-- <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->

        <h1>Hello World</h1>
        <!-- 2 way binding -->
        <input type="text" v-model="user">
        <!-- 1 way binding -->
        <h1 class="myClass">Hey!! {{ user }}</h1>
    </div>
</template>

<script>

export default {
    data() {
        return {
            //let user = " "
            user: "Abhi"
        }
    },
}
</script>

<style>
.myClass {
    color: red;
}
</style>
