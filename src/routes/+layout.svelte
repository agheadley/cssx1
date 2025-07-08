<script lang="ts">
	import '../normalize.css';
	import '../app.css';

	let { children } = $props();
</script>

<div class="app">
	<header>
		<div>Header here!</div>
		<div>and here!</div>
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
		border-bottom:1px solid var(--font);
		position:fixed;
		min-width:100%;
		background:#fff;
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		align-items: center;
		margin:0;
		padding:1rem;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		margin: 5rem auto;
		box-sizing: border-box;
		border:0px solid green;
	}

	footer {
		border-top:1px solid var(--font);
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		margin:0;
		min-width:100%;
		
	}

	
</style>
