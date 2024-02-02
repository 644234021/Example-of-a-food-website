<template>
    <div>
      <h3>เมนู : {{ drink.Name }}</h3>
      <p>ราคา: {{ drink.Price }} บาท</p>
      <p :class="{ 'bold-red-text': drink.DrinkType === 'เครื่องดื่มแอลกอฮอล์' }">ประเภท: {{ drink.DrinkType }}</p >
      <!-- แก้ src ให้เรียกไฟล์รูปภาพแบบถูกต้อง -->
      <img :src= "'src/assets/drinkImage/'+drink.ImageFile" :alt="drink.Name" /> 
      
    </div>
  </template>
  
  <script>
  export default {
    props: {
      drink: Object,
    },
  };
  </script>
  
  <style scoped>
  .bold-red-text {
    font-weight: bold;
    color: red;
  }
  
  div{
      background-color: rgb(192, 243, 252);
    }
  </style>
  