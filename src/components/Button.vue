<template>
<button @click="onClick()"  :style="{background: color}" class="btn btn-click">{{text}}</button>

</template>
<script>
export default {
    name: 'Button',
    props:{
        text:String,
        color:String
    },
    methods:{
        onClick(){
             this.$emit('btn-click')
        }
    }
}
</script>
