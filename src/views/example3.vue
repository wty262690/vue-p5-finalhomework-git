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
  <audio controls>
  <source src="https://raw.githubusercontent.com/himalayasingh/music-player-1/master/music/2.mp3" type="audio/ogg">
  <source src="https://raw.githubusercontent.com/himalayasingh/music-player-1/master/music/2.mp3" type="audio/mpeg">
</audio>
<audio controls>
  <source src="https://raw.githubusercontent.com/wty262690/vue-p5-finalhomework-git/main/src/sound/ranbow_newyear.mp3" type="audio/mpeg">
</audio>
  <div class="container">
    <div class="Canvas"></div>
    </div>
</template>

<script>
import $ from 'jquery'
export default {
  data() {  
    
    return {
    trackUrl : ['../sound/ranbow_newyear.mp3',],  
    }
    
  },
methods: {
 playSound (sound) {
      if(sound) {
        var audio = new Audio(require(trackUrl));
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