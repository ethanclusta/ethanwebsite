<script>
	import '../app.css';
    import NavItem from '../lib/NavItem.svelte';

	const pages = ['articles', 'film', 'code'];
</script>

<div class="mx-20 mt-10 text-3xl font-bold">Ethan Corcoran</div>
<hr class="mx-20" />
<h1 class="text-zinc-600 mx-20 mb-10">
	{#each pages as pg (pg)}
		<NavItem name={pg} />
		{#if pg !== 'code'}/{/if}
	{/each}
</h1>

<div class="mx-20">
	<slot />
</div>
