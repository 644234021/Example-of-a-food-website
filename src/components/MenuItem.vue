<template>
  
    <div>
      <h3 >เมนู : {{ menu.Name }}</h3>
      <p>ราคา: {{ menu.Price }} บาท</p>
      <p>โปรตีน : {{ menu.Protein }}</p>
      <p>แคลอรี่ : {{ menu.Calories }}</p>
      <img :src= "'src/assets/MenuImage/'+menu.ImageFile" :alt="menu.Name" /> 
      
    </div>
  </template>
  
  <script>
  export default {
    props: {
      menu: Object,
    },
  };
  </script>
  
  <style scoped>
    div{
      background-color: rgb(192, 243, 252);
    }
  </style>
  