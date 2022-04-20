<script>
export default {
    data(){
        return{
        button_text: "text"
        }
    },
    methods:{
        transition(){
            this.button_text="transitioned!"
        }
    }
}
</script>


<template>
    <button @click="transition">{{button_text}}</button>
</template>
