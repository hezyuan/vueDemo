<template>
  <div class="hello">
    <input type="button" value="你好啊我是来测试的"  @click="button1"/>
    <h2 >{{testTitle}}</h2>
    <test-component :test3="test4" ref="testcomponent"></test-component>
    <test-component1></test-component1>
  </div>
</template>

<script>
  import TestComponent from './TestComponent'
  import TestComponent1 from './TestComponent1'
export default {
  name: 'HelloWorld',
  components:{
    TestComponent,
    TestComponent1,
  },
  data () {
    return {
      test4:"8858558585888",
      testTitle:"",
    }
  },

  mounted(){
    let _this=this;
    drag.$on('testClick', function (a) {
      _this.testTitle=a;
    })
  },

  methods:{
      button1(){
        this.$refs['testcomponent'].test2();
      }
  }


}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
