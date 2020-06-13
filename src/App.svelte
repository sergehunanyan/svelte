<script>
	import Header from './Header.svelte';
	import Footer from './Footer.svelte';
	import Product from './Product.svelte';
</script>

<div class="content">
	<Header/>
	<div class="products_list">
		<ul>
			<Product/>
			<Product/>
			<Product/>
			<Product/>
			<Product/>
			<Product/>
		</ul>
	</div>
	<Footer/>
</div>

<style>
	.products_list{
		padding: 15px;
		display: flex;
		flex-direction: column;
		align-items: flex-end;
		margin: 130px 0 80px;
	}
	ul{
		list-style: none;
		margin: 0;
		padding: 0;
		width: 100%;
	}
</style>