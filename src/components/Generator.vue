<script>
    export default {
        data () {
            return {
                counter: [],
            } 
        },
        methods: {

            generator(){
                this.counter.push(Math.floor(Math.random() * 100))
            
            }
        },
    }
</script>

<template>
    <div class="block-gen">
        <h3>{{ counter[counter.length - 1] }}</h3>
        <button @click="generator">rundom nimbers</button>
        <p>{{ counter }}</p>
    </div>
</template>

<style scoped>
    .block-gen{
        display: flex;
        flex-direction: column;
        align-items: center;
        margin-top: 30px;
    }
    button{
        width: 120px;
        height: 50px;
        background-color: rgb(145, 145, 145);
        color: white;
        border-radius: 3px;
        font-size: 20px;
    }
    h3{
        color: rgb(128, 128, 128);
        font-size: 35px;
    }
    p{
        color: rgb(145, 145, 145);
        font-size: 30px;
    }
</style>