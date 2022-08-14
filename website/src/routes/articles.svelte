<script>
	import Article from '../lib/Article.svelte';

	const articles = [
		{
			name: 'ESCAPE THE ALGORITHM',
			url: 'https://turtlesdown.substack.com/p/escape-the-algorithm'
		},
		{
			name: "HOW'S THE WEATHER?",
			url: 'https://turtlesdown.substack.com/p/hows-the-weather'
		},
		{
			name: 'IS THE WEB THE SAME AS THE BOOK?',
			url: 'https://turtlesdown.substack.com/p/is-the-web-the-same-as-the-book'
		},
		{
			name: 'WHY TURTLES?',
			url: 'https://turtlesdown.substack.com/p/why-turtles'
		},
		{
			name: 'ARE YOU ENGAGED YET?',
			url: 'https://turtlesdown.substack.com/p/are-you-engaged-yet'
		},
		{
			name: 'HISTORY OR MEMORY?',
			url: 'https://turtlesdown.substack.com/p/history-or-memory-an-exploration'
		}
	];
</script>

<svelte:head>
	<title>EC | Articles</title>
</svelte:head>

<p class="lg:w-1/2">
    I write a newsletter called Turtles on the thoughts I have while researching digital media and culture.
    You can subscribe <a target="_blank" class="text-blue-600 underline" href="https://turtlesdown.substack.com">here</a> or check out my articles below.
</p>
<div class="lg:w-1/2 mb-10">
	{#each articles as article}
		<Article details={article} />
	{/each}
</div>
