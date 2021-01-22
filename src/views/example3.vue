<template>
  <button class="btn btn-primary btn-sm" @click.prevent="playSound('../sound/ranbow_newyear.mp3')">  
  <p>沒</p>
  <p>人</p>
  <p>能</p>
  <p>在</p>
  <p>我</p>
  <p>的</p>
  <p>BGM</p>
  <p>裡</p>
  <p>戰</p>
  <p>勝</p>
  <p>我</p></button>
  <audio src="../sound/ranbow_newyear.mp3"></audio>
  <div class="container">
    <div class="Canvas"></div>
    </div>
</template>

<script>
export default {
  data() {  
    
    return {
      
    }
  },
methods: {
    playSound (sound) {
      if(sound) {
        var audio = new Audio(require('../sound/ranbow_newyear.mp3'));
        audio.play();
      }
    }
  },

}
</script>

<style>
#app{
  text-align: center;
}
</style>