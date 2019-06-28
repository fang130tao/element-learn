<template>
  <div id="app">
      <el-button @click="show = !show">Click Me</el-button>
      <div style="display: flex; margin-top: 20px; height: 100px;">
          <transition name="el-fade-in-linear">
              <div v-show="show" class="transition-box">.el-fade-in-linear</div>
          </transition>
          <transition name="el-fade-in">
              <div v-show="show" class="transition-box">.el-fade-in</div>
          </transition>
          <transition name="el-zoom-in-center">
              <div v-show="show" class="transition-box">.el-zoom-in-center</div>
          </transition>

          <transition name="el-zoom-in-top">
              <div v-show="show" class="transition-box">.el-zoom-in-top</div>
          </transition>

          <transition name="el-zoom-in-bottom">
              <div v-show="show" class="transition-box">.el-zoom-in-bottom</div>
          </transition>
      </div>
      </div>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    // HelloWorld

  },
  data(){
    return{
      show: true
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.transition-box {
    margin-bottom: 10px;
    width: 200px;
    height: 100px;
    border-radius: 4px;
    background-color: #409EFF;
    text-align: center;
    color: #fff;
    padding: 40px 20px;
    box-sizing: border-box;
    margin-right: 20px;
}
</style>
