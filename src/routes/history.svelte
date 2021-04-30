<script>
	import history from './history';
</script>

<svelte:head>
	<title>Work History</title>
</svelte:head>


	<h1 class="heading font-semibold">Work History</h1>
	{#each history as h}
		<h3 class="font-semibold">
			{h.title}, <a href={h.urls[0]}> <span style="font-style: italic;">{h.company}</span></a>
			<span style="float:right">{h.start} - {h.end} </span>
		</h3>
		<ul class= "my-4 ml-6 text-sm list-disc list-outside ">
			{#each h.highlights as i}
				<li class="">{i}</li>
			{/each}
		</ul>
	{/each}


<style>
	.heading {
		margin-bottom: 50px;
	}
</style>
