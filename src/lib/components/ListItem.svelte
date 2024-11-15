<script>
	export let icon, title, index;
	let ABC = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ';
</script>

<button class="alert flex focus:outline focus:outline-primary">
	{#if icon}
		<img src={icon} alt={title + '-Icon'} />
	{:else}
		<span>{ABC[index]}</span>
	{/if}
	<span>{title}</span>
</button>
