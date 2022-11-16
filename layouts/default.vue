<template>
	<div>
		<div v-if="$nuxt.isOffline" class="flex justify-center py-8 text-2xl font-semibold text-red-400">
			Your connection has been interrupted. You are offline
		</div>
		<Menu />
		<Nuxt/>
	</div>
</template>