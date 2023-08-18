<script setup lang="ts">
import TheWelcome from '../components/TheWelcome.vue'


import openioe from 'openioe';

openioe.weather({
  cityName:"辽宁 沈阳",  //必传
  //time:'2022-05-26',  //可选。默认为当前日期
  success:function(result){  //成功回调
      console.log(result)
  },
  error:function(status){
    console.log(status)
  }
})

</script>

<template>
  <main>
    <TheWelcome />
  </main>
</template>
