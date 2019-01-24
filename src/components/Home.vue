<template>
 <div>
     <h2>这是一个新的组件</h2>
     <ul>
       <li v-for="(item,index) in datalist" :key='index'>{{item.personName}}</li>
     </ul>
     <hr>
 </div>
</template>

<script>
 export default {
   data () {
     return {
       datalist:[]
     }
   },
   mounted(){
     this.showData()
   },
   methods:{
     showData(){
       this.$http.get('/user').then((res)=>{
         this.datalist = res.data.data
       }).catch((err)=>{
         console.log('c')
       })
     }
   },
 }
</script>

<style scoped>
h2{
    color: brown;
}
 
</style>
