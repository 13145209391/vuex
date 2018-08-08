<template>
  <div id="productsone">
    <h2> Products List One</h2>
	<ul>
		<li v-for="product in products">
			<span class="name">{{product.name}}</span>
			<span class="price">${{product.price}}</span>
		</li>
	</ul>
  </div>
</template>

<script>

export default {
  props:["products"],
  components: {
		
  }
}
</script>

<style scoped>
	#productsone{
		background:skyblue;
		padding:40px;
	}
	
</style>
