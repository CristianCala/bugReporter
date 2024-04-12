<template>
	<div v-if="loading" class="flex items-center justify-center h-screen">
		<div
			class="inline-block h-8 w-8 animate-spin rounded-full border-4 border-solid border-current border-e-transparent align-[-0.125em] text-primary motion-reduce:animate-[spin_1.5s_linear_infinite]"
			role="status"
		>
			<span
				class="!absolute !-m-px !h-px !w-px !overflow-hidden !whitespace-nowrap !border-0 !p-0 ![clip:rect(0,0,0,0)]">Loading...</span>
		</div>
	</div>
	<div v-else class="flex min-h-full flex-col justify-center px-6 py-12 lg:px-8 mt-32">
		<div class="mt-10 sm:mx-auto sm:w-full sm:max-w-sm bg-white p-4 rounded-lg shadow-lg">
			<div class="sm:mx-auto sm:w-full sm:max-w-sm bg-white">
				<h2 class="mt-5 text-center text-2xl font-black leading-9 tracking-tight text-gray-900">Login</h2>
				<p class="mt-2 text-center text-sm text-gray-600 max-w">
					A report bug system for projects
				</p>
			</div>
			<form class="space-y-6" action="#" method="POST">
			<div>
				<div class="mt-2">
					<input
						id="email"
						name="email"
						type="email"
						placeholder="Email/Username"
						autocomplete="email"
						required
						class="block w-full rounded-md px-2 py-1.5 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6"
					>
				</div>
			</div>

			<div>
				<div class="mt-2">
					<input
						id="password"
						name="password"
						type="password"
						autocomplete="current-password"
						placeholder="Contraseña"
						required
						class="block w-full rounded-md px-2 py-1.5 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6"
					>
				</div>
			</div>

			<div>
				<button type="submit" class="flex w-full justify-center rounded-md bg-indigo-600 px-3 py-1.5 text-sm font-semibold leading-6 text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">Sign in</button>
			</div>
			</form>

			<p class="mt-2 text-center text-sm text-gray-500">
				- Or sign in with -
			</p>
			<p class="mt-1 text-center text-sm text-gray-500">
				<a href="#" class="font-semibold leading-6 text-indigo-600 hover:text-indigo-500 rounded-md px-3 py-1.5 border border-grey">
					<ion-icon name="logo-google" class="mr-1"></ion-icon>
					Google
				</a>
			</p>
			<p class="mt-5 text-center text-sm text-gray-500">
				Dont have an account?
			<a href="#" class="font-semibold leading-6 text-indigo-600 hover:text-indigo-500">Create one here</a>
			</p>
		</div>
	</div>
</template>

<script>
export default {
    name: 'HomeView',
	data() {
		return {
			loading: false
		}
	},
}
</script>
