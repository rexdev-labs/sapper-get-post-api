<script>
	import Nav from '../components/Nav.svelte';

	export let segment;
</script>

<style>
	main {
		position: relative;
		max-width: 100%;
		min-height: 100vh;
		background-color: white;
		padding: 2em;
		background-color: rgb(211, 211, 211);
		margin: 0 auto;
		box-sizing: border-box;
	}
</style>

<Nav {segment}/>

<main>
	<slot></slot>
</main>