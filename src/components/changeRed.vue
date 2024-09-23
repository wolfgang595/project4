  <script>
  //simple method to color red
  export default {
    methods: {
      changeColor() {
        this.$emit('change-color', 'red');
      }
    }
  }
  </script>
  



<!-- button to change color -->
  <template>
    <button @click="changeColor">Red</button>
  </template>
  




<!-- style of button -->

  <style scoped>
  button {
    background-color: red;
    color: white;
    padding: 10px;
    border: none;
    cursor: pointer;
  }
  </style>
  