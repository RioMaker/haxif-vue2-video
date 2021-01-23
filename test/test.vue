<template>
  <div class="test">
    <haxifVideo title="标题">
      <source src="../assets/海浪30.mp4">
    </haxifVideo>
  </div>
</template>

<script>
import haxifVideo from '../src/Video.vue';
export default {
  components: { haxifVideo },
  data(){
    return{
      
    }
  }
}
</script>

<style scoped>
.test{
  width: 120vw;
  height: 100vh;
  display: flex;
  justify-content: center;
}
</style>
