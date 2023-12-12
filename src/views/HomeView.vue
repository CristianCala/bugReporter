<template>
	<div class="flex items-center justify-center h-screen">
		<div class="max-w-sm rounded overflow-hidden shadow-lg">
			<div class="px-6 py-4 text-center">
				<div class="font-bold text-2xl mb-2">Welcome to Bug Reporter</div>
				<p class="text-gray-900">
					A report bug system for projects
				</p>
				<router-link
					to="/projects"
					class="bg-black text-white rounded-md font-bold py-2 px-28 mt-4 inline-block hover:bg-gray-700"
				>
					Get Started
				</router-link>
			</div>
		</div>
	</div>
</template>

<script>
export default {
    name: 'HomeView',
    data() {
        return {
            message: 'Hello World!'
        }
    }
}
</script>
