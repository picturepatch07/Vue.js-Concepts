<template>
    <div class="home">
        <h1>Welcome to Home page</h1>
        <input type="text" v-model="fname" placeholder="Enter firstname">
        <input type="text" v-model="lname" placeholder="Enter lastname">
        <h1>Fullname: {{ fullName }}</h1>
    </div>
</template>

<script>

export default {
    data() {
        return {
            fname: "",
            lname: "",
            fullName: ""
        }
    },
    watch: {
        fname(newValue, oldValue){
            this.fullName = newValue+ ' '+this.lname
        },
        
    }
}
</script>