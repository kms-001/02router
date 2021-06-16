<template>
  <top-header />

  <router-view :listData="listData"></router-view>



  <bottom-footer />
</template>

<script>
import header from './components/header.vue'
import footer from './components/footer.vue'
import listData from './listData.js'

export default {
  name:'app',
  components:{
     'top-header':header,
     'bottom-footer':footer,
  },
  data(){
    return{
      listData:listData,
    }
  }
}
</script>

<style>

</style>