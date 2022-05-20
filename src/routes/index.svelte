<script context="module" lang="ts">
	export const prerender = true;
</script>

<script lang="ts">
	import Tab from '$lib/Tab.svelte';
</script>


<section>

	<Tab />

</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}

</style>
