<script>
import PropsTest from './components/PropsTest.vue'
// import PropsTest from '@/components/PropsTest.vue'
import {ref,reactive, } from 'vue'
export default {
  components:{
    PropsTest,
  },
  setup(props) {
    const str = ref('Hello daisy!')

    const bool = ref(true)

    const num = ref(0)

    const arr = reactive([])

    const obj = reactive({})

    const handclickfn = () => {

    }
    return{
      str, 
      bool,
      num,
      arr,
      obj,
      handclickfn
    }
  }
}
</script>
  
<template>
  <PropsTest 
    :str="str" 
    :bool="bool"
    :num="num"
    :arr="arr"
    :obj="obj"
    :handclickfn="handclickfn"
  />
</template>

<style >
#app {
  /* font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale; */
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
