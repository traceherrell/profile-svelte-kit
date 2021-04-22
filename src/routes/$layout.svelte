<script>
	import Nav from '$lib/Nav/Nav.svelte';


</script>

<style>
	main {
		position: relative;
		max-width: 56em;
		background-color: white;
		padding: 2em;
		margin: 0 auto;
		box-sizing: border-box;
	}
</style>
<head>
	<script src="https://kit.fontawesome.com/98f378dec0.js" crossorigin="anonymous"></script>
	<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">

</head>
<Nav />

<main>
	<slot></slot>
</main>