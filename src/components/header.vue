<template>
    <header>
        <h1>Bear's Gallery</h1>
    </header>
</template>

<script>

export default{
    name: 'Header',
    components: {  
    },
}

</script>

<style scoped>
    Header{
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 10px;
        padding: 10px;

    }
    h1{
       margin-left: auto; 
       margin-right: auto;
    }
</style>

