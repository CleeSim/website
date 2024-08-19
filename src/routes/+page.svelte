<script>
	// import FaLinkedin from 'svelte-icons/fa/FaLinkedin.svelte';
	import FaGithub from 'svelte-icons/fa/FaGithub.svelte';
	import FaEnvelope from 'svelte-icons/fa/FaEnvelope.svelte';
	// import FaMedium from 'svelte-icons/fa/FaMedium.svelte';
	import { modalOpened } from '$lib/store';
</script>

<svelte:head>
	<title>CleeSim</title>
	<link href="https://fonts.googleapis.com/css2?family=Kanit&display=swap" rel="stylesheet">
</svelte:head>

<main>
	<h1 class="title">CleeSim</h1>
	<h2 class="desc-text">We're an independent Roblox game development team.</h2>
	<div class="icons">
		<div
			role="button"
			tabindex="0"
			on:keypress={() => {
				modalOpened.set(true);
			}}
			on:click={() => {
				modalOpened.set(true);
			}}
		>
			<div class="icon">
				<FaEnvelope />
			</div>
		</div>

		<a
			href="https://github.com/CleeSim"
			aria-label="GitHub"
			target="_blank"
			rel="noopener noreferrer"
		>
			<div class="icon">
				<FaGithub />
			</div>
		</a>
	</div>
</main>

<style>
	a {
		color: white;
		text-decoration: none;
	}

	main {
		text-align: center;
		padding: 0;
		margin: 0 auto;

		display: flex;
		flex-direction: column;
		height: calc(100vh - 80px - 88px);
		justify-content: center;
		align-items: center;
	}

	h1 {
		font-weight: 700;
    text-shadow: 0 0 10px #b3b3b3, 0 0 20px #b3b3b3, 0 0 30px #b3b3b3, 0 0 40px #a6a6a6;
	}

	main > h1 {
		margin: 50px 10px 0;
		font-size: 36px;
	}

	.icons {
		display: flex !important;
		align-items: center;
		gap: 20px;
		cursor: pointer;
		font-size: 30px;
		justify-content: space-between;
		max-width: 200px;
		margin: 50px auto 0;
	}

	.icon {
		cursor: pointer;
		transition: color 0.2s ease-in-out;
		width: 40px;
	}

  .title {
      font-size: 84px;
      margin-bottom: 50px;
      font-family: 'Kanit', sans-serif;
  }

	.icon:hover {
		color: #ca3c25;
	}

	@media (min-width: 900px) {
		main > h1 {
			font-size: 48px;
			font-family: 'Kanit', sans-serif;
		}
	}

	@media (min-width: 600px) {
		main {
			max-width: none;
			font-family: 'Kanit', sans-serif;
			font-weight: 500;
		}
	}
</style>
