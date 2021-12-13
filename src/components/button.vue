<template>
    <button @click="onClick()" :style="{
        background: color}" class="btn">{{ text }}
    </button>
</template>

<script>
export default{
    name: 'Button',
    props: {
        text: String,
        color: String,
    },
    methods:{
    onClick(){
        window.location.href = "mailto:ktobin1@bu.edu";
    },
    }
}
</script>

<style scoped>
button{
    margin: 15px;
}
button.btn{
    margin-left: auto;
    margin-right: auto;
}
</style>