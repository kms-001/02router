<template>
  <h1>logo</h1>
  <ul class="menu clearfix">
      <!-- <li v-for="(a,i) in menu" :key="i"> {{a}} </li> -->
      <!-- <li><router-link to="/">home</router-link></li>
      <li><router-link to="/company">company</router-link></li>
      <li><router-link to="/product">product</router-link></li> -->

      <li v-for="(item,i) in menu" :key="i">
          <router-link :to="menu[i].link"> {{menu[i].title}} </router-link>
      </li>
  </ul>
</template>

<script>
export default {
    name:'header',
    data(){
        return{
            menu:[
                {title:'home',link:'/'},
                {title:'company',link:'/company'},
                {title:'product',link:'/product'}
            ],
        }
    }
}
</script>

<style>

</style>