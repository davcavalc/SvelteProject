<script>
	import {Router, Route} from 'svero';
	import Header from './Header.svelte';
	import Index from './Header.svelte';
	import About from './Header.svelte';
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>

<style>
	
</style>

<Header/>

<div class="container">

	<Router>
		<Route path='*' component={Index} />
		<Route path='/About' component={About} />
		<Route path='*' component={Index} />
		
	</Router>

</div>
