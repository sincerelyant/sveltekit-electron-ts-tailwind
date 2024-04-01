<script lang="ts">
	export let text: string;
	export let extraClass: string = '';
</script>

<button
	on:click
	class="{extraClass} rounded-md bg-red-500 px-8 py-2 text-lg uppercase text-white duration-100 ease-in-out hover:bg-red-600"
	>{text}</button
>
