<template>

  <div class="outer">
    <div class="before"></div>
      <div class="inner">
        <div class="title" v-if='"{{ $route.params.id }}"'>{{ $route.params.id }}</div>
        <div class="title" v-else>Oh no 😢</div>
      </div>
  </div>


</template>



<script>




export default {
  name: 'Hero',
  props: {
    msg: String
  }
}
</script>



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .outer{
    width: 100%;
    height: 65vh;
    background-color: #f4f4f4;
    position: relative;
    z-index: 1;
     object-fit: cover;
    background-repeat: no-repeat;
    background-position: bottom; 
    background-image: url('https://spheracinema.com/sites/default/files/styles/large_image/public/38846132282_ec5acbfb55_o.jpg');
  }

  .inner{
    font-size: 80px;
    font-weight: bolder;
    color: white;
    z-index: 10;
    width: 100%;
    height: 100%;
    position: absolute;
    left: 0;
    top: 0;
    display: grid;
    place-items: center;
  }

  .title{
    font-variant-numeric: tabular-nums;
  }

  .title .thin{
    font-weight: lighter;
    margin-left: -20px;
  }

  .before{
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    background-color: #1d2633;
    opacity: .5;
    z-index: 2;
  }
</style>
