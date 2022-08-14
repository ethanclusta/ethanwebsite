<script>
import Video from "../lib/Video.svelte";

    const urls = [
        "https://player.vimeo.com/video/561892850?h=aabe03ca1f&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479",
        "https://player.vimeo.com/video/561882631?h=93f6f87eb3&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479",
        "https://player.vimeo.com/video/561884077?h=c0337e93b8&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479",
    ]
</script>

<svelte:head>
	<title>EC | Film</title>
</svelte:head>

<p class="lg:w-1/2">
    The films I write and direct explore a range of themes, including perception, national identity and so on.
    But mostly I'm just trying to make them a fulfilling experience to watch. You can find some of my personal favourites below.
</p>
<div class="lg:w-1/2 mb-10">
	{#each urls as url }
        <Video url={url} />
    {/each}
</div>
