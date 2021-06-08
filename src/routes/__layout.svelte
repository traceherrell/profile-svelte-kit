<script>
	import Nav from '$lib/Nav/Nav.svelte';
	import '../app.postcss';
</script>

<head>
	<script src="https://kit.fontawesome.com/98f378dec0.js" crossorigin="anonymous"></script>
		<link rel="preconnect" href="https://fonts.gstatic.com" />
	<link
		href="https://fonts.googleapis.com/css2?family=Open+Sans&family=Roboto:wght@100;300;400&display=swap"
		rel="stylesheet"
	/></head
>
<Nav />
<main class="max-w-4xl p-8 mx-auto ">
	<slot />
</main>

<style>
</style>
