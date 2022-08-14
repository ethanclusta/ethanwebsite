<script>
	export let details;
</script>

<a target="_blank" href={details.url}>
	<div
		class="mt-10 relative w-full bg-rose-500 shadow-xl hover:shadow-2xl transition duration-300 ease-in-out"
	>
		<div class="ml-2 text-white font-bold text-7xl">{details.name}</div>
	</div>
</a>
