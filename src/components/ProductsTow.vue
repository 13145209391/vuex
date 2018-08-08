<template>
  <div id="productstow">
    <h2> Products List Tow</h2>
	<ul>
		<li v-for="product in products" :key="product.id">
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
	#productstow{
		background:peachpuff;
		padding:40px;
	}
</style>
