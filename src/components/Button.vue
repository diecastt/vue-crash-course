<template>
    <button @click = "onClick()" :style = "{backgroundColor: color}" class="btn">
    {{ text }}
    </button>
</template>

<script>
import { TypedChainedSet } from 'webpack-chain';

export default {
    name: 'Button',
    props: {
        text: String,
        color: String,
    },
    methods: {
        onClick(){
            this.$emit('btn-click')
        },    
    }
}
</script>

<style>
    
</style>