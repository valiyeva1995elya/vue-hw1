<script>
    export default {
        data() {
            return {
                counter: 0
            }
        },
        methods: {
            like() {
                this.counter++
            }
        }
    }
</script>

<template>
    <div class="block-likes">
        <button @click="like">♥</button>
        <p>{{ counter }}</p>
    </div>
</template>

<style scoped>
    .block-likes{
        color: rgb(147, 146, 146);
        display: flex;
        justify-content: center;
        align-items: center;
        margin-top: 30px;
        font-size: 30px;
    }
    button{
        background-color: rgb(145, 145, 145);
        color: white;
        width: 60px;
        height: 30px;
        border: none;
        border-radius: 3px;
        font-size: 25px;
        margin-right: 20px;
    }
</style>