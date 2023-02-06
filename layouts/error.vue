<template>
	<div>
		<div class="py-36 flex justify-center items-center flex-col">
			<div class="mb-12">
				<h1 v-if="error.statusCode === 404" class="text-4xl textPrim">Page not found</h1>
				<h1 v-else class="text-4xl textPrim">An error occurred</h1>
			</div>
			<NuxtLink to="/" class="px-6 py-1 rounded-xl bg-red-400 hover:bg-red-300">Home page</NuxtLink>
		</div>
		
	</div>
  </template>
  
  <script>
	export default {
	  props: ['error'],
	  layout: 'error'
	}
  </script>