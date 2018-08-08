<template>
  <div id="app">
    <ones :products="products"></ones>
		<tows :products="products"></tows>
  </div>
</template>

<script>
import ProductsOne from './components/ProductsOne.vue'
import ProductsTow from './components/ProductsTow.vue'
export default {
  name: 'App',
  components: {
		'ones':ProductsOne,
		'tows':ProductsTow
  },
	data(){
		return{
			products:[
				{name:"马云",price:"100"},
				{name:"马化腾",price:"90"},
				{name:"马冬梅",price:"60"},
				{name:"马容",price:"10"}
			]
		}
	}
}
</script>

<style>
	body{
		font-family:Ubuntu;
		color:#000;
	}
	ul li{
		list-style-type: none;
		color:#fff;
		font-weight:bold;
		padding:10px;
		background:olive;
		margin:10px 0;
	}
</style>
