<script>
	import Logo from '$lib/assets/Logo.png';
	import Louche from '$lib/assets/Louche.png';
</script>

<svelte:head>
	<link
		href="https://fonts.googleapis.com/css2?family=Khand:wght@300;400;500;600;700&display=swap"
		rel="stylesheet"
	/>
</svelte:head>

<div class="info">
	<h1 class="hidden">La Cabane Val-David</h1>
	<img src={Logo} alt="Logo de La Cabane" class="logo mb-10" />
	<div class="soon mb-10">
		<img src={Louche} alt="" />
		<h2 class="title_soon ml-5 text-6xl font-light">Coming soon...</h2>
	</div>
	<div class="contact">
		<h3>Contact ___</h3>
		<address class="pl-12 not-italic">1505 rue le familial, Val-David, Québec</address>
		<a href="tel:+819 325 3305" class="pl-12">(819) 325-3305</a>
	</div>
</div>

<div class="credit text-slate-800">
	<p>crédit photo : Laeticia Gaillet 'Des soupes qui nous font du bien' - éditions La Plage</p>
</div>

<style lang="postcss">
	:global(body) {
		background-color: whitesmoke;
		background-image: url('$lib/assets/IMG_Soup2.png');
		background-repeat: no-repeat;
		background-size: cover;
	}

	.info {
		position: relative;
		top: 21vh;
		left: 14%;

		display: flex;
		flex-direction: column;
		/* align-items: center; */
		width: 25%;

		font-family: Khand;
	}

	.soon {
		display: flex;
		align-items: center;
	}

	.credit {
		position: absolute;
		bottom: 1%;
		right: 1%;

		font-size: 0.4rem;
	}
</style>
