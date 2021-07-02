<script>
	import profile from '../../static/profile_standing.jpg';
	import Button from '$lib/Button.svelte';

	const scrollTo = (e) => {
		console.log('got it');
		e.stopPropagation();

		if (window) {
			window.scrollTo({
				top: 700,
				left: 100,
				behavior: 'smooth'
			});
		}
	};
</script>

<svelte:head>
	<title>Trace Herrell</title>
</svelte:head>

<header class="container">
	<div class="flex flex-wrap">
		<!-- Grid column -->
		<div class="w-full   lg:w-1/2">
			<!-- Column contents -->
			<img alt="Profile" src={profile} class="img-responsive" />
		</div>
		<!-- Grid column -->
		<div class="w-full pt-8  lg:w-1/2">
			<!-- Column contents -->
			<h2 class="text-7xl font-medium ">Hello, I'm Trace</h2>
			<p class=" text-2xl font-light py-4 leading-7  ">
				A Software Engineer from the Pacific North West, Seattle area. Want to know more about me?
			</p>
			<Button text="Read More" on:click={scrollTo} />
			<a class="text-blue-600 underline mx-4" href="https://www.linkedin.com/in/traceherrell/">
				<i class="fa fa-lg fa-linkedin" />
			</a>
		</div>
	</div>
</header>

<section class="section about-me pt-24">
	<div class="container">
		<h1 class="pb-8">About Me</h1>
		<div>
			<p>
				I have several years of experience building end to end solutions in a variety of verticals:
				healthcare, insurance, e-commerce, real estate, education, and IoT. I am competent engineer
				and dev manager comfortable in all areas of the software stack. In the last few years I have
				really used my experience to help organizations build right sized, scalable, and
				maintainable solutions often during times of technical transformations. As an Azure
				certified solution architect and certified scrum master I bring years of experience to
				leading teams and designing/building new capabilities.
			</p>
		</div>
		<div>
			<p>
				As a lifelong learner, I'm always fascinated by new technologies and different approaches to
				software engineering. I've created this profile site several times, most recently with React
				and Vue. This time I chose to use a new framework called <a
					class="text-blue-600 underline"
					href="https://svelte.dev/"
				>
					Svelte</a
				>. And even though I am Azure certified this site is hosted on Google Cloud Platform.
			</p>
			<p>
				I'm using Svelte's server-side rendering framework called SvelteKit. Conceptually, this is
				like Angular Universal and React's NextJS, where node servers like express are used to
				render components on the first call to the server. After the application is loaded in the
				browser, it uses service workers to pre fetch content and fully hydrate the application.
				Svelte is different from both of React and Vue in that it does not use a runtime nor virtual
				dom. It compiles all the code at build time. Here is the link to the
				<a href="https://github.com/traceherrell/profile-svelte-kit"> source.</a>
			</p>
			<p />
		</div>
		<div class="flex flex-wrap pt-16 interest">
			<div class="w-full   lg:w-1/4">
				<h2>
					<i class="fab  fa-react" /> React
				</h2>
				<p>
					I've built a couple of projects as well as leading new end teams. Redux state management,
					story book components
				</p>
			</div>
			<div class="w-full   lg:w-1/4">
				<h2>
					<i class="fab fa-vuejs" /> Vue
				</h2>
				<p>
					Introduced Bluetooth to Vue and led the adoption state management (Vuex) as a design
					pattern.
				</p>
			</div>
			<div class="w-full   lg:w-1/4">
				<h2>
					<i class="fab  fa-microsoft" /> .Net Core
				</h2>
				<p>Micro services. Queues, Event Sourcing, Repository, Dependency injection.</p>
			</div>
			<div class="w-full   lg:w-1/4">
				<h2>
					<i class="fab fa-docker" /> Docker
				</h2>
				<p>Azure container services (ACS), Azure Kubernetes Service (AKS), Azure DevOps.</p>
			</div>
		</div>

		<div class=" w-full flex flex-wrap pt-8 interest">
			<div class="w-full   lg:w-1/4">
				<h2>
					<i class="fa fa-lg fa-html5" /> HTML/CSS
				</h2>
				<p>
					Implement responsive designs for a usable experience across desktop, tablet, and phone
					browsers.
				</p>
			</div>
			<div class="w-full   lg:w-1/4">
				<h2>
					<i class="fa fa-lg fa-code" /> Code
				</h2>
				<p>
					Well versed in functional and OO programming. I primarily write JavaScript, and C#.
					Recently new to Rust
				</p>
			</div>
			<div class="w-full   lg:w-1/4">
				<h2>
					<i class="fa fa-lg fa-cloud" /> API
				</h2>
				<p>
					Develop RESTful interfaces that incorporate stateless designs, self-descriptive messages
					and semantic URLs. Apigee, Azure Api Management.
				</p>
			</div>
			<div class="w-full   lg:w-1/4">
				<h2 class="sub-heading">
					<i class="fa fa-lg fa-database" /> Database
				</h2>
				<p>
					Relational, Document, Azure SQL Server, Cosmos, Mongo, Redis, T-SQL, Modeling, Query
					optimization.
				</p>
			</div>
		</div>
	</div>
</section>

<style style lang="postcss">
	.about-me p {
		margin-bottom: 20px;
		font-size: 1.1em;
	}

	.interest p {
		font-size: 1em;
	}
</style>
