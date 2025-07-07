<script lang="ts">
	import '../normalize.css';
	import '../app.css';

	let { children } = $props();
</script>

<div class="app">
	<header>
		<p>Header here!</p>
	</header>

	<main>
		{@render children()}
	</main>

	<footer>
		<p>
			visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to learn about SvelteKit
		</p>
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
		padding:0;
	}

	header {
		border:0px solid red;
		border-bottom:1px solid 
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
		border:0px solid green;
	}

	footer {
		border:1px solid gray;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		margin:0;
		min-width:100%;
		
	}

	
</style>
