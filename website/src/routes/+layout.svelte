<script lang="ts">
	import '../app.css';
	import favicon from '$lib/assets/favicon.svg';
	import topBg from '$lib/assets/top-bg.png';
	import bottomBg from '$lib/assets/bottom-bg_upscayl_2x_upscayl-standard-4x.png';
	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<div class="relative h-screen w-full bg-[#F6F3E5]">
	<img
		class="pointer-events-none fixed bottom-0 left-0 w-full opacity-100 select-none"
		alt="flower background"
		src={bottomBg}
	/>
	{@render children()}
</div>
