<template>
  <div>
    <snow></snow>
    <lights></lights>
    <br><br><br><br>
    <span>
      <h2>Chistams is in</h2>
      <no-ssr>
      <Countdown deadline="December 25, 2018"></Countdown></no-ssr>
    </span>
    <snowman></snowman>
  </div>
</template>

<script>
  import snowman from '~/components/snowman.vue'
  import lights from '~/components/lights.vue'
  import Countdown from 'vuejs-countdown'
  import snow from '~/components/snow.vue'

  export default {
    components: {
      Countdown,
      snowman,
      lights,
      snow
    }

  }

</script>

<style>
  body {
    margin: 0;
    padding: 0;
    overflow: hidden;
  }

  span {
    display: inline-block;
    text-align: center;
    width: 100vw;
    color: white;
  }

  span h2 {
    padding-right: 10px;
    
  }

</style>
