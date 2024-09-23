  <script>
  //simple method to color green
  export default {
    methods: {
      changeColor() {
        this.$emit('change-color', 'green');
      }
    }
  }
  </script>
  





  <template>
    <button @click="changeColor">Green</button>
  </template>
  




  <style scoped>
  button {
    background-color: green;
    color: white;
    padding: 10px;
    border: none;
    cursor: pointer;
  }
  </style>
  