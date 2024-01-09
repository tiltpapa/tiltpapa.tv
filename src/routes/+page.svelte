<script>
    import { each } from "svelte/internal";

	const links = [
		{"label": "Twitter","href": "https://x.com/texiruto3"},
		{"label": "Nostr","href": "https://nostter.app/tiltpapa.tv"},
		{"label": "Bluesky","href": "https://bsky.app/profile/tiltpapa.tv"},
		{"label": "Mastodon","href": "https://mstdn.jp/@tiltpapa"}
	];
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="ティル父さん" />
</svelte:head>

<section>
	<h1>ティル父さん</h1>
	{#each links as link}
		<li>
			<a href="{link.href}">{link.label}</a>
		</li>
	{/each}
</section>

<style>

</style>
