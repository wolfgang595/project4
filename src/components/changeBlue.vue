  <script>
  //simple method to color blue
  export default {
    methods: {
      changeColor() {
        this.$emit('change-color', 'blue');
      }
    }
  }
  </script>
  





  <template>
    <button @click="changeColor">Blue</button>
  </template>
  






  <style scoped>
  button {
    background-color: blue;
    color: white;
    padding: 10px;
    border: none;
    cursor: pointer;
  }
  </style>
  