<template>
  <div>
    <div class="blank"></div>
    <div class="wrapper">
      <div class="img1"></div>
      <h2 class="title1">lorem ipsum <br><span>aaaaaa</span></h2>
      <div class="img2"></div>
      <h2 class="title2">lorem ipsum <br>  aaaaaa</h2>
    </div>
    <div class="blank"></div>
  </div>
</template>
<script>

import { gsap } from 'gsap'

export default {
  mounted: function (){
    this.startAnimations()
  },
  methods: {
    startAnimations: function(){
      gsap.to('#title',{duartion: 1, color:'red'})
    }
  }

}
</script>


<style>
  *{
    padding: 0;
    margin: 0;
  }
  .blank{
    height: 100vh;
    width: 100%;
  }

</style>
