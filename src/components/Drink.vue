<template>
    <div>
      <div v-for="drink in drinkData" :key="drink.DrinkId">
        <DrinkItem :drink="drink" />
      </div>
    </div>
</template>
  
<script>
  import DrinkItem from './DrinkItem.vue';
  
  export default {
    data() {
      return {
        drinkData: [
          {
            "DrinkId": 1,
            "Name" : "ชาเขียวมัทฉะ",
            "Price" : 100,
            "DrinkType" : "เครื่องดื่มที่ไม่มีแอลกอฮอล์",
            "ImageFile" : "01.jpg"
          },
          {
            "DrinkId": 2,
            "Name" : "ชาซากุระ",
            "Price" : 110,
            "DrinkType" : "เครื่องดื่มที่ไม่มีแอลกอฮอล์",
            "ImageFile" : "02.jpg"
          },
          {
            "DrinkId": 3,
            "Name" : "มัทฉะลาเต้",
            "Price" : 150,
            "DrinkType" : "เครื่องดื่มที่ไม่มีแอลกอฮอล์",
            "ImageFile" : "03.jpg"
          },
          {
            "DrinkId": 4,
            "Name" : "ยาคูลท์",
            "Price" : 20,
            "DrinkType" : "เครื่องดื่มที่ไม่มีแอลกอฮอล์",
            "ImageFile" : "04.jpg"
          },
          {
            "DrinkId": 5,
            "Name" : "สาเก",
            "Price" : 500,
            "DrinkType" : "เครื่องดื่มแอลกอฮอล์",
            "ImageFile" : "05.jpg"
          },
          {
            "DrinkId": 6,
            "Name" : "โชจู",
            "Price" : 400,
            "DrinkType" : "เครื่องดื่มแอลกอฮอล์",
            "ImageFile" : "06.jpg"
          },
          {
            "DrinkId": 7,
            "Name" : "ไวน์บ๊วยอูเมะชุ",
            "Price" : 300,
            "DrinkType" : "เครื่องดื่มแอลกอฮอล์",
            "ImageFile" : "07.jpg"
          }
        ]
      };
    },
    components: {
      DrinkItem
    }
  };
</script>
  
<style>
  
</style>
  