<template>
  <h1>{{title}}</h1>
</template>

<script>
    export default {
        name: "TestComponent1",
        data(){
          return{
            title:"",
          }
        },
        mounted(){
          drag.$on('testClick8',(a)=>{
            this.title=a;
          })
        }
    }
</script>

<style scoped>

</style>
