<template>
    <header>
        <h1>{{ title }}</h1>
        <Button @click="onClick()" text="Add task" color="green" />
    </header>
</template>

<script>
import Button from './Button'

export default {
    name: 'Header',
    props: {
        title: String,
    },
    components:{
        Button
    },
    methods: {
        onClick(){
            console.log('click')
        }
    }
}
</script>

<style scoped>
    header{
        display: flex;
        align-content: center;
        justify-content: space-between;
    }
</style>