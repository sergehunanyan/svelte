<script>

</script>

<header>
	<div class="header_top">
		<button>
			<img src="images/header/search.png" alt="Search">
		</button>
		<a href="#">
			<img src="images/header/heart.png" alt="Wishlist">
		</a>
	</div>
	<div class="header_bottom">
		<ul>
			<li class="active">Popular</li>
			<li>Pizza</li>
			<li>Salads</li>
			<li>Hot meals</li>
			<li>Drinks</li>
			<li>Deserts</li>
			<li>Sauces</li>
		</ul>
	</div>
</header>

<style>
	header{
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		z-index: 999;
		background-color: rgba(255, 255, 255, .95);
	}
	.header_top{
		display: flex;
		justify-content: space-between;
		align-content: center;
		flex-wrap: wrap;
		border-bottom: 1px solid #e0e0e0;
		padding: 10px 15px;
		background-color: transparent;
	}
	button{
		background-color: transparent;
		border: none;
	}
	img{
		width: 40px;
		height: auto;
	}

	ul{
		list-style: none;
		margin: 20px 15px 0;
		padding: 0 0 20px;
		display: flex;
		overflow: auto;
	}
	li{
		border: 1px solid #80cb4b;
		border-radius: 50px;
		padding: 6px 20px;
		margin-right: 10px;
		color: #80cb4b;
		background-color: transparent;
		font-size: 13px;
		white-space: nowrap;
	}
	li.active{
		background-color: #80cb4b;
		color: #ffffff;
		box-shadow: 3px 4px 8px #80cb4b;
	}

	@media all and (max-width: 480px) {
		img{
			max-width: 20px;
		}
	}
</style>