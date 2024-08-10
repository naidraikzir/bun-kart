<script lang="ts">
	import { cartStore } from '$lib/stores/cart.svelte';

	let { children } = $props();
</script>

<div style="margin-bottom: 10px;">
	<a href="/">Products</a>
	<a href="/cart">🛒 Cart ({cartStore.totalItems})</a>
</div>

{@render children()}
