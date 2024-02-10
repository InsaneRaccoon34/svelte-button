<script>
</script>

<section class="container">
	<a class="button"> This Is A BUTTON </a>
</section>

<style lang="scss">
	$border-radius: 0.5rem;
	$text-color: black;

	.container {
		height: 80vh;
		width: 100%;
		display: grid;
		place-items: center;
	}

	.button {
		position: relative;
		padding: 3rem 5rem;
		outline: $orange 2px solid;
		border-radius: $border-radius;
		font-size: 2rem;
		cursor: pointer;

		color: $orange;
		transition: 0.3s;
		transition-property: color transform;

		&::after {
			content: '';
			position: absolute;
			left: 0;
			bottom: 0;
			border-radius: $border-radius;

			background-color: #f5900b;

			height: 0;
			width: 100%;

			z-index: -1;

			transition: all 0.5s;
		}

		&:hover {
			color: white;
			transform: scale(1.1);
      box-shadow: 10px 10px 8px -4px rgba(0, 0, 0, 0.75);
			&::after {
				border-radius: $border-radius;
				height: 100%;
				width: 100%;
			}
		}
	}
</style>
