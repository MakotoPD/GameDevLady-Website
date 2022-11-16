<template>
	<header class="flex justify-between px-8 pt-8 z-50">
		<div class="flex items-center space-x-6">
			<nuxt-img src="/logo.png" placeholder sizes="sm:60px md:60px"/>
			<p class="text-lg font-bold text-red-400">GameDevLady</p>
		</div>
		<div class="flex items-center space-x-6">
			
			<nav class="hidden md:flex space-x-12 font-bold mr-4">
				<nuxt-link to="/materialy" class="text-gray-500 ">Materiały</nuxt-link>
				<nuxt-link to="/o-mnie" class="text-gray-500 ">O mnie</nuxt-link>
				<nuxt-link to="/kontakt" class="text-gray-500 ">Kontakt</nuxt-link>
			</nav>
			<button class="ml-4 p-2 md:hidden">
				<nuxt-img src="/hamburger.svg" placeholder />
			</button>

		</div>
	</header>
</template>

