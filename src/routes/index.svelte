<script>
	import Counter from '$lib/Counter.svelte';
</script>

<main>
	<p>this is index.svelte, please navigate to another page to reproduce the bug</p>
	<h3>Reproducing steps:</h3>
<ol>
    <li>click on "1"</li>
    <li>URL changes, content of page "one" is displayed</li>
    <li>on page "1" click on "2"</li>
    <li>URL changes, content stays to page "one"s content</li>
    <li>on page "2" click on "3"</li>
    <li>URL changes, content stays to page "one"s content</li>
</ol>
</main>

<style>
	:root {
		font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell,
			'Open Sans', 'Helvetica Neue', sans-serif;
	}

	main {
		text-align: center;
		padding: 1em;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4rem;
		font-weight: 100;
		line-height: 1.1;
		margin: 4rem auto;
		max-width: 14rem;
	}

	p {
		max-width: 14rem;
		margin: 2rem auto;
		line-height: 1.35;
	}

	@media (min-width: 480px) {
		h1 {
			max-width: none;
		}

		p {
			max-width: none;
		}
	}
</style>
