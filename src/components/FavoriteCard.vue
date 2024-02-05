<template>
	<div class="container">
		<div><img :src="cardData.imgSrc" class="img" alt="">
		</div>
		<div class="shop">
			<img :src="cardData.imgMiniSrc" class="imgShop" alt="">
			<div>{{ cardData.titleShop }}</div>
		</div>
		<div class="title">{{ cardData.title }}</div>
	</div>
</template>

<script>
export default {
	name: 'FavoriteCard',
	props: {
		cardData: {
			type: Object,
			default: () => ({})
		},
	},
}
</script>

<style lang="css" scoped>
.container {
	display: inline-block;
	
}

.img {
	width: 150px;
}

.imgShop {
	width: 80px;
}

.shop {
	display: flex;
}

.title {
	font-size: 14px;
	text-align: left;
}
</style>	