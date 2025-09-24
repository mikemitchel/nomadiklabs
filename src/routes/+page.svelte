<script>
	import logo from '$lib/assets/logo.svelte';
</script>

<div class="container">
	<div class="box">
		<svelte:component this={logo} />
		<div class="name">NOMADIK LABS</div>
	</div>
	<div class="tag">All that is gold does not glitter,</div>
	<div class="tag">Not all who wander are lost.</div>
	<div class="tag">The old that is strong does not wither,</div>
	<div class="tag">Deep roots are not reached by the frost.</div>
	<br />
	<div class="tag">~J.R.R Tolkien</div>
</div>
<footer>
	<p class="copyright">© 2024-2025 Nomadik Labs LLC. All rights reserved</p>
</footer>

<style>
	:global(body) {
		background-image: url($lib/assets/sunset.jpeg);
		background-position: center center;
		background-repeat: no-repeat;
		background-attachment: fixed;
		background-size: cover;
		background-color: #fff4de;

		min-height: 100vh;
		display: flex;
		flex-direction: column;
		overflow: hidden;
	}

	.container {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.box {
		margin: 10vh;
		display: flex;
		align-items: center;
		flex-direction: row;
	}

	.name {
		margin: 10px;
		font-family: Tahoma, Arial, Helvetica, sans-serif;
		font-weight: bold;
		font-size: 6vmin;
		color: #172830;
	}

	.tag {
		display: flex;
		justify-content: center;
		margin: 10px;
		font-family: Tahoma, Arial, Helvetica, sans-serif;
		font-style: italic;
		font-size: 3vmin;
		color: #fff4de;
	}

	.copyright {
		font-family: Tahoma, Arial, Helvetica, sans-serif;
		color: #fff4de;
	}

	p.copyright {
		margin-bottom: 15px;
		font-size: 3vmin;
	}

	footer {
		display: flex;
		justify-content: center;
		margin-top: auto;
	}
</style>
