
<script>
export default {
    props:{
        str:{
            type:String,
            default:"Daisy~妳沒有傳遞props進來"
        },
        bool:{
            type:Boolean,
            default: true,
        },
        num:{
            type:Number,
            default:0,
        },
        arr:{
            type:Array,
            default: () => [],
        },
        obj:{
            type: Object,
            default: () => ({}),
        },
        handclickfn:{
            type:Function,
            default:() => {},
        }
    },
    setup(props) {
        console.log(props);
        return{ props, }
    }
}
</script>

<template >
    <h1>{{props.str}}</h1>
</template>

<style lang="scss">
    h1{
        color:red;
        font-size: 50px;
        
    }
</style>