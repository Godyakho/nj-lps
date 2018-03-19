<!-- ******************************************
*  Author : niuzz niuzz@hotmail.com
*  Created On : Mon Mar 12 2018
******************************************* -->
<template>
	<div class="basewidth">
		<author></author>
		<newslist></newslist>
	</div>
</template>

<script type="text/ecmascript-6">
import author from 'components/author.vue'
import newslist from 'components/newslist.vue'
export default {
	data: () => ({
		message: 'Layout VUE is here!!!!'
		}),
	components: {
		author,
		newslist
    },
	created: function() {
		this.$(function() {
			console.log('-----------------------')
			console.log('this is created')
			console.log('-----------------------')	
		})
	}
}
</script>

<style lang="scss" scoped>
@media screen and (min-width: 500px) {
    .basewidth {
		width: 1100px;
		margin: 0 auto
    }
}

</style>
