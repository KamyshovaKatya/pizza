<template>
  <div id="app">
   <app-pizza v-bind:pizzaName='pizzaName' v-bind:pizzaSize='pizzaSize' v-bind:pizzaPrice='pizzaPrice'>
<h1 slot="n1">Покупайте пиццу!</h1>
<p>Состав: мука, соль, перец, томатная паста, колбаса, сыр</p>
   </app-pizza>
  </div>
</template>

<script>
import Pizza from './components/Pizza.vue'

export default {
  name: 'app',
  data(){
    return {
      pizzaName: 'ШПицца от Школы программистов',
      pizzaPrice: 600,
      pizzaSize: 30
    }
  },
  components: {
    appPizza: Pizza
  } 
}
</script>

<style>
body {
    background: rgb(238,174,202);
    background: radial-gradient(circle, rgba(238,174,202,1) 0%, rgba(148,187,233,1) 100%);
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    margin: 0;
    padding: 0;
    font-family: sans-serif;
    font-size: 18px;
}
</style>