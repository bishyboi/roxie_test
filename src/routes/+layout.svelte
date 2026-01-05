<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link
	href="https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=Instrument+Serif:ital@0;1&display=swap"
	rel="stylesheet"
/>
<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}

<style>
    :global(body) {
        margin: 0;
        padding: 0;
        width: 100%;
        background-color: #818c7e;
    }

    :global(html){
        scroll-behavior: smooth;
    }
</style>
