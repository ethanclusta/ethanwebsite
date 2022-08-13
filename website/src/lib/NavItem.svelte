<script>
	import { page } from '$app/stores';

	export let name;

	const space = ' ';
	const navStyle = 'text-zinc-800 hover:text-rose-500 transition duration-150 ease-in-out';
	const selNavStyle = 'text-rose-500 transition duration-150 ease-in-out';
</script>

{#if $page.url.pathname !== `/${name}`}
	<a class={navStyle} href="/{name}">
		{#if name === 'articles'}
			{name}
		{:else if name === 'code'}
			{space}{name}
		{:else}
			{space}{name}{space}
		{/if}
	</a>
{:else}
	<a class={selNavStyle} href="/{name}">
		{#if name === 'articles'}
			{name}
		{:else if name === 'code'}
			{space}{name}
		{:else}
			{space}{name}{space}
		{/if}
	</a>
{/if}
