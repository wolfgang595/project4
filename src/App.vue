<script>
import changeRed from './components/changeRed.vue';
import changeGreen from './components/changeGreen.vue';
import changeBlue from './components/changeBlue.vue';


export default {
  components: {
    changeRed,
    changeBlue,
    changeGreen,
  },
  data() {
    return {
      backgroundColor: 'white'
    };
  },
  methods: {
    changeBackgroundColor(color) {
      this.backgroundColor = color;
    }
  }
}
</script>






<template>



  <div :style="{ backgroundColor: backgroundColor }" class="app-container">

    <h1>Welcome, please choose a color to change the background</h1>


    <changeRed @change-color="changeBackgroundColor" />
    <changeGreen @change-color="changeBackgroundColor" />
    <changeBlue @change-color="changeBackgroundColor" />
  </div>
</template>



<style>
.app-container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  flex-direction: column;
}
</style>
