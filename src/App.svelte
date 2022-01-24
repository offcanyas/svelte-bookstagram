<script>
	import Book from './Book.svelte';

	let books = [
		{ id: 1, 
			author: 'Dave Eggers',
			title: 'Every',
			img: 'img/every.jpg',
			date: '07.10.2021'
		},
		{ id: 2, 
			author: 'Simon Sinek',
			title: 'The Infinite Game',
			img: 'img/infinite-game.jpg',
			date: '2019'
		},
		{ id: 3,
			author: 'Antje Rávik Strubel',
			title: 'Blaue Frau',
			img: 'img/blaue-frau.jpg',
			date: '2021'	
		}
	];
</script>

<style>
	.book__container {
		max-width: 930px;
		margin: 0 auto;
		display: flex;
		flex-direction: column;
		align-items: center;
	}
</style>

<div class="book__container">
	{#each books as book}
		<Book 
			author={book.author}
			title={book.title}
			img={book.img}
			date={book.date}
		/>
	{/each}
</div>