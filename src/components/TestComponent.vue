<template>
  <div>
  <input type="button" value="我是来取传过来的值看看" @click="test2" />
  <input type="button" value="把A传给B" @click="test8" />
    <h2>{{test3}}</h2>
  </div>
</template>

<script>
    export default {
        name: "TestComponent",
      props:{
        test3:String,
      },
      data(){
        return{
          msg: '看一看',
          test3:"",
          msg8:"兄弟传值",
        }
      },

      mounted(){

      },

      methods:{
        test2(){
          drag.$emit('testClick',this.msg);
          console.log(this.msg);
          let _this=this;
          _this.test3=this.test3;
          console.log("=="+this.test3);
        },
        test8(){
          drag.$emit('testClick8',this.msg8);
        }
      },
    }
</script>

<style scoped>

</style>
