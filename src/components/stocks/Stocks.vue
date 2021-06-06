<template>
  <v-layout row wrap>
    <Stock v-for="stock in stocks" :key="stock.id" :stock="stock" />
  </v-layout>
</template>

<script>
import Stock from './Stock'
export default {
  components: {Stock},
  data(){
    return{
      stocks: [
        {id: 1, name: 'BTS Card', price: 120},
        {id: 2, name: 'BlackPink Card', price: 80},
        {id: 3, name: 'TxT Card', price: 100},
        {id: 4, name: 'ITZY Card', price: 95},
      ]
    }
  }
}
</script>

<style>

</style>