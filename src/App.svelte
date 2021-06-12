<script>
	let cats = [
		{ id: 'J---aiyznGQ', name: 'Кот на клавишных' },
		{ id: 'z_AbfPXTKms', name: 'Мару' },
		{ id: 'OUtn3pvWmpg', name: 'Экзистенциальный кот' }
	];
</script>

<h1>Знаменитые YouTube котики</h1>

<ul>
	{#each cats as cat}
		<li><a target="_blank" href="https://www.youtube.com/watch?v={cat.id}">
			{cat.name}
		</a></li>
	{/each}
</ul>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
		text-align:center;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}

	li {
		text-align:center;
		font-size:2em;
	}
</style>