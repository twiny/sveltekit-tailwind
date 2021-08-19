<script context="module">
	export function load({ error, status }) {
		return {
			props: {
				error: error,
				status: status
			}
		};
	}
</script>

<script>
	export let error;
	export let status;
</script>

<!--  -->
<svelte:head>
	<title>Something wrong | NameAuditor</title>
	<meta name="robots" content="noindex nofollow" />
	<html lang="en" />
</svelte:head>

<div class="flex h-screen bg-gray-100 justify-items-center">
	<!-- This file lives in public/404.html -->
	<div class="container m-auto px-4">
		<section class="py-8 px-4 text-center">
			<div class="max-w-auto mx-auto">
				<div class="md:max-w-lg mx-auto text-9xl font-bold">
					{status}
				</div>
				<h2 class="mt-8 uppercase text-xl lg:text-5xl font-black">
					We are sorry, Somthing went wrong!
				</h2>
				<p class="mt-6 uppercase text-sm lg:text-base text-gray-900">
					{error.message}
				</p>
				<a
					href="/"
					class="mt-6 bg-blue-500 hover:bg-blue-700 text-white font-light py-4 px-6 rounded-full inline-block uppercase shadow-md"
					>Back To Homepage</a
				>
			</div>
		</section>
	</div>
</div>
