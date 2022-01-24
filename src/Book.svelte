<script>
  export let img;
	export let author;
  export let title;
  export let date;
</script>

<style>
  .book {
    margin-right: 20px;
    border: 1px solid #eee;
    box-shadow: 0 0 20px #88888815;
    width: 100%;
    padding: 20px 20px 10px;
    margin-bottom: 30px;
  }

  .book__image {
    margin: 0 auto;
    display: block;
    max-width: 200px;
  }

  .font-bold {
    font-weight: 600;
  }

</style>

<section class="book">
	<img class="book__image" src="{img}" alt="{author} - {title}" title="{author} - {title}" />
  <p class="book-info">
    <span class="font-bold">Autor:</span> {author} <br />
    <span class="font-bold">Titel:</span> {title}<br />
    <span class="font-bold">Erscheinungsdatum:</span> {date}
  </p>
</section>