<script>
</script>

<section class="container">
	<a class="button">This Is A BUTTON</a>
</section>

<style lang="scss">
	.container {
    height: 80vh;
    width: 100%;
    display: grid;
    place-items: center;
	}

  .button {
    // container
    padding: 1rem 1rem;
    outline: $orange 2px solid;
    border-radius: 2px;

    // text
    color: $orange;

    // behaviour
    transition: all 50ms ease;
  }
</style>
