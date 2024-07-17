<!-- <script setup>
	const route =  useRoute()
	const id = route.params.id
</script>


<template>
	<div>
<h1>ID : {{ id }}</h1>
	</div>
</template> -->

<script setup>
definePageMeta({
	middleware: [
		function (to) {
			if (to.params.id === '1')
				return navigateTo('/')
			if (to.params.id === '2')
				return abortNavigation()
			if (to.params.id === '3')
				return abortNavigation('id should not be 3')
		}
	]
})

</script>


<template>
	<div>

		<!-- <h1>ID : {{ $route.params.id }}</h1> -->
	</div>
</template>




<style lang="scss" scoped></style>