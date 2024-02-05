<template>
	<div>
		<favorite-card v-for="card in cardsListData" :key="card.id" :card-data="card"></favorite-card>
	</div>
</template>

<script>
import FavoriteCard from "./FavoriteCard.vue";
export default {
	name: 'FavoritePanel',
	props: {
		cardsListData: {
			type: Array,
			default: () => []
		},
	},
	components: { FavoriteCard }
}
</script>

<style lang="css" scoped>

</style>