<script>
	import Button from '$lib/Button.svelte';
    import ButtonLink from '$lib/ButtonLink.svelte'
	import ls1 from './launchstudio.png';
	import jls1 from './j_search.png';
	let open = false;
	const toggle = () => (open = !open);
    const navigate = () => {
       
        window.location.href =  "portfolio/bluetooth";
    }
    const navigateJLS= () => {
        window.location.href =  "https://www.johnlscott.com/search";
    }
</script>

<svelte:head>
	<title>Trace Herrell - Portfolio</title>
</svelte:head>



<div class="container px-5 py-24 mx-auto">
	<div class="flex flex-wrap -mx-4 -mb-10 ">
		<div class="sm:w-1/2 mb-10 px-4">
			<div class="rounded-lg h-64 overflow-hidden">
				<img alt="content" class="object-cover  h-full w-full" src={ls1} />
			</div>
			<h2 class="title-font text-2xl font-medium mt-6 mb-3">
				Bluetooth Launch Studio
			</h2>
			<p class="leading-relaxed text-base">
				A tool to complete the Bluetooth qualification process. This tool is only for bluetooth
				members so I can't link directly to the application. Click below to view some screens.
			</p>
			<Button text="View Screen Shots" on:click={navigate }></Button>
		</div>
		<div class="sm:w-1/2 mb-10 px-4">
			<div class="rounded-lg h-64 overflow-hidden">
				<img alt="content" class="object-cover object-center h-full w-full" src={jls1} />
			</div>
			<h2 class="title-font text-2xl font-medium  mt-6 mb-3">John L Scott</h2>
			<p class="leading-relaxed text-base pb-7">
				Search and find real estate listings similar to Redfin and Zillow. Since this is a public
				site you can click the button below to try it out yourself.
			</p>
			<a class="flex-shrink-0 
            text-white 
            bg-gray-500 
            border-0 py-2 
            px-8 focus:outline-none 
            hover:bg-gray-600 
            rounded 
            text-lg 
            mt-10 
            sm:mt-0" href='https://www.johnlscott.com/search'>JohnLScott.com</a>
		</div>
	</div>
</div>
