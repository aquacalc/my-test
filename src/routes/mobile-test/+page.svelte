<script>
	//
</script>

<div class="container">
	<div class="img-left">
		<img
			class="my-img"
			id="service-img"
			src="naomi-hebert-MP0bgaS_d1c-unsplash.jpg"
			alt="hero kitchen"
		/>
		<div class="service-text">
			<h2 class="my-h2 text-center text-blue-800">Real Estate Done Right</h2>
			<p class="my-para text-balance leading-8 text-gray-500">
				Nervous about your property adventure? Don’t be. Whether you're getting ready to buy or
				sell, in the middle of it, or just looking for some answers, our top-notch skills ensure you
				get the best experience possible. It’s what we love to do.
			</p>
		</div>
	</div>

	<div class="img-right">
		<div class="service-text">
			<h2 class="my-h2 text-center text-blue-800">Yadda</h2>
			<p class="my-para text-balance leading-8 text-gray-500">
				Nervous about your property adventure? Don’t be. Whether you're getting ready to buy or
				sell, in the middle of it, or just looking for some answers, our top-notch skills ensure you
				get the best experience possible. It’s what we love to do.
			</p>
		</div>
		<img
			class="my-img"
			id="service-img"
			src="naomi-hebert-MP0bgaS_d1c-unsplash.jpg"
			alt="hero kitchen"
		/>
	</div>
</div>

<!-- <p>
	For Mobile Devices – 320px — 480px. iPads and Tablets – 481px — 768px. Laptops and small screen –
	769px — 1024px. Large screens and Desktops – 1025px — 1200px.
</p> -->

<style>
	.container {
		display: grid;
		margin: 20px auto;
		max-width: 1200px;
		gap: 1rem;
		/* justify-content: center;
		align-items: center; */

		/* item with flexible width but a minimum of 200 pixels. */
		/* >= 200px && <= 1fr */
		/* grid-template-columns: repeat(auto-fill, minmax(200px, 1fr)); */
	}

	.img-left {
		display: flex;
		flex-direction: column;
	}

	.img-right {
		display: flex;
		flex-direction: column-reverse;
	}

	.my-img {
		display: block;
		width: 70vw;
		margin: 30px auto;
		margin-bottom: 8px;
    aspect-ratio: auto 1 / 1;
	}

	.my-h2 {
		font-size: 1.5rem;
		font-weight: 700;
	}

	#service-img,
	#service-img-2 {
		/* width: 300px;
			margin: 0 auto; */
		border-radius: 8px;
		box-shadow:
			0px 1px 2px 0px rgba(0, 0, 0, 0.2),
			1px 2px 4px 0px rgba(0, 0, 0, 0.2),
			2px 4px 8px 0px rgba(0, 0, 0, 0.2),
			2px 4px 16px 0px rgba(0, 0, 0, 0.2);
	}

	.service-text {
		padding: 4px;
    margin: 10px;
    
	}

	/* MEDIA */

	@media (min-width: 640px) {
		.container {
			/* grid-template-columns: repeat(2, 1fr); */
			grid-template-rows: repeat(2, 1fr);
			gap: 2rem;
		}

		.img-left,
		.img-right {
      /* flex: 110; */
			flex-direction: row;
		}

		.my-img {
			width: 50vw;
			margin: 1rem;
		}

		.my-para {
			font-size: 1rem;
			/* margin-right: 0.85rem; */
		}
	}

	@media (min-width: 768px) {
		.container {
			/* grid-template-columns: repeat(3, 1fr); */
			gap: 0;
		}

		.my-img {
			width: 45vw;
			margin-left: 1.5rem;
		}

		.my-h2 {
			font-size: 1.5rem;
			font-weight: 700;
		}

		.service-text {
			padding: 30px;
			margin-right: 10px;
		}

		.my-para {
			font-size: 1.25rem;
		}
	}

	@media (min-width: 1024px) {
		/* .container {
			grid-template-columns: repeat(3, 1fr);
		} */

		.my-img {
			width: 40vw;
		}

		.my-h2 {
			font-size: 1.95rem;
		}

		.service-text {
			padding: 25px;
			margin-right: 50px;
		}

		.my-para {
			font-size: 1.45rem;
		}
	}

	@media (min-width: 1200px) {
		/* .container {
			grid-template-columns: repeat(3, 1fr);
		} */

		.my-img {
			width: 35vw;
		}

		.my-h2 {
			font-size: 2.2rem;
		}

		.service-text {
			padding: 25px;
			margin-right: 20px;
		}

		.my-para {
			font-size: 1.5rem;
		}
	}

	/* @media (min-width: 640px) {
	} */

	/* @media (min-width: 768px) {
	} */

	/* @media (min-width: 1024px) {
	} */

	/* @media (min-width: 1200px) {
	} */
</style>
