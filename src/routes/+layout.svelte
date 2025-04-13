<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>

<div class="fixed inset-0 w-full h-full bg-cover bg-center -z-10" style="background-image: url('/images/gutter-hero.png');"></div>
<div class="fixed inset-0 w-full h-full bg-black/60 -z-10"></div>

<main class="relative z-0">
	{@render children()}
</main>
