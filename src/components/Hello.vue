<template>
  <!-- <div class="hello">
    <h1>{{ msg }}</h1>
    <p>{{ detail }}</p>
      <input v-model="detail">
  </div> -->
  <div id="vue_det" class="hello">
    <h1>site : {{ site }}</h1>
    <h1>url : {{ url }}</h1>
    <!-- <h1>Alexa : {{ created() }}</h1> -->
    <h1>{{ detail }}</h1>
    <label for="r1">ÐÞ¸ÄÑÕÉ«</label><input type="checkbox" v-model="use" id="r1">
    <br><br>
    <div v-bind:class="{ 'class1': use }">
      v-bind:class Ö¸Áî
    </div>
    <br><br>
    <p id="demo"> time:</p>
    <button type="button" onclick="displayData">time</button>
  </div>
</template>

<script type="text/javascript">
import Vue from 'vue'
/* eslint-disable no-new */
export var data = { site: 'QT', url: 'www.runoob.com', alexa: 10000 }
export var vm = new Vue({
  el: '#vue_det',
  data: data,
  methods: {
    details: function () {
      return this.site + '2664'
    // },
    // displayData: function () {
    //   document.getElementById('vue_det').innerHTML = Date()
    }
  }
})

export default {
  name: 'hello',
  data () {
    return {
      msg: 'Hello world vue.js',
      detail: 'Fanva',
      url: 'www.runoob.com',
      use: false,
      methods: {
        func: function () {
          return this.msg
        }
      }
    }
  },
  created: function () {
    alert(2 * 3)
  },
  displayData: function () {
    document.getElementById('demo').innerHTML = Date()
  }
}

document.write(vm.$data === data)
document.write('<br>')
vm.site = 'Runoob'
document.write(data.site + '<br>')
data.alexa = 1234
document.write(vm.alexa + '<br>')
document.write(vm.$el === document.getElementById('vue_det'))
document.write('<br>' + vm.details())
</script>

<style>
.class1 {
  background: #444;
  color: #eee;
}
</style>
