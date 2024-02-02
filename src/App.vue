<template>
  <div id="app">
    <h1>รายการอาหาร</h1>
    <Menus v-if="menuData" :menus="menuDataData" />
    <br><h1>รายการเครื่องดื่ม</h1>
    <Drink v-if="drinkData" :drinks="drinkData" />
  </div>
</template>

<script>
import Menus from './components/Menu.vue';
import menuData from './data/Menu.json';
import Drink from './components/Drink.vue';
import drinkData from './data/Drink.json';

export default {
  data() {
    return {
      menuData: menuData,
      drinkData: drinkData,
    };
  },
  components: {
    Menus,
    Drink,
  },
};
</script>

<style>
  #app{
    background-color: rgb(240, 247, 244);
  }
  h1{
    text-shadow: 2px 2px #999;
    background-color: rgb(250, 248, 128);
    padding: 0.1%;
  }
  

</style>