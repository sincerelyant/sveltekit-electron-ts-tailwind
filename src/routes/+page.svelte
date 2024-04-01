<script lang="ts">
	import SuccessButton from '$lib/success-button.svelte';
	import DangerButton from '$lib/danger-button.svelte';

	let count = 0;

	// actions
	const increment = () => count++;
	const decrement = () => count--;
	const reset = () => (count = 0);
</script>

<div class="mt-20 space-y-5 text-center">
	<h1 class="text-4xl font-semibold uppercase">hello world</h1>
	<p class="text-lg uppercase">sveltekit + electron + typescript + tailwind</p>
	<p class="text-lg font-semibold uppercase">count : {count}</p>
	<div class="mx-auto grid max-w-sm grid-cols-2 gap-2">
		<SuccessButton text="increment" on:click={increment} />
		<SuccessButton text="decrement" on:click={decrement} />
		<DangerButton text="reset" extraClass="col-span-2" on:click={reset} />
	</div>
</div>
