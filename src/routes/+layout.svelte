<script>
	import { dev } from '$app/environment';
	import { injectAnalytics } from '@vercel/analytics/sveltekit';

	injectAnalytics({ mode: dev ? 'development' : 'production' });

	import '../app.css';
</script>

<nav class="mb-10 bg-gray-100 fixed top-0 left-0 right-0 z-50">
	<a href="/" title="My Guy Bri HOME">
		<img class="py-1" id="my-guy-bri-img" src="my-guy-bri-logo.jpg" alt="hero kitchen" />
	</a>
	<!-- <div class="nav-links text-gray-500 hidden md:flex"> -->
	<div class="nav-links text-gray-500">
		<a href="/#about-me" title="About Brian">Meet Brian</a>
		<!-- <a href="#search-homes" title="Search properties">Search</a> -->
		<!-- <a href="#our-services" title="My services">Services</a> -->
		<a href="/endorsements" title="Results">Results</a>
		<a href="/#contact-me" title="Contact Brian">Contact</a>
	</div>
</nav>

<slot />

<style>
	.container {
		width: 100%;
		height: 100vh;
		margin: 70px auto;
	}

	nav {
		display: grid;
		grid-template-columns: 1fr 3fr;
		align-items: center;
	}

	#my-guy-bri-img {
		width: 100px;
		border-radius: 15px;
		margin-left: 1rem;
	}

	.nav-links {
		display: flex;
		padding-left: 2rem;
		align-items: center;
	}

	.nav-links a {
		font-size: 0.85rem;
		color: #041e42;
		opacity: 0.5;
	}

	.nav-links a:hover {
		cursor: pointer;
		opacity: 1;
	}

	section {
		display: flex;
		flex-direction: column;
		align-items: center;
		gap: 1.5rem;
	}

	#hero-img {
		width: 80vw;
		border-radius: 8px;
		box-shadow:
			0px 1px 2px 0px rgba(0, 0, 0, 0.2),
			1px 2px 4px 0px rgba(0, 0, 0, 0.2),
			2px 4px 8px 0px rgba(0, 0, 0, 0.2),
			2px 4px 16px 0px rgba(0, 0, 0, 0.2);
	}

	button {
		border-radius: 22px;
		padding: 20px;
		width: 80%;
		border: 1px solid #041e42;
		color: #041e42;
		opacity: 0.85;
		font-weight: 500;
		font-size: 1.65rem;
		margin-bottom: 50px;

		/* transition: background-color 2s; */
		transition:
			color,
			background-color 1.5s;
	}
	button:hover {
		background-color: #041e42;
		color: #fff;
		/* opacity: 1; */
	}

	.my-hr {
		display: flex;
		align-items: center;
		margin-top: 30px;
	}

	.hr-1,
	.hr-2 {
		border: 1px lightgray solid;
		margin: 0px;
		flex: 1 1 0;
	}

	/* ABOUT */
	.about-brian {
		margin: 0 auto;
		width: 80%;
	}

	/* -- ** -- SERVICES -- ** -- */

	.services {
		display: grid;
		gap: 3rem;
	}

	.row-1,
	.row-2 {
		display: flex;
		flex-direction: column;
		text-align: center;
		gap: 1rem;
	}

	.row-2 {
		flex-direction: column-reverse;
	}

	#service-img,
	#service-img-2 {
		width: 80vw;
		margin: 0 auto;
		border-radius: 8px;
		box-shadow:
			0px 1px 2px 0px rgba(0, 0, 0, 0.2),
			1px 2px 4px 0px rgba(0, 0, 0, 0.2),
			2px 4px 8px 0px rgba(0, 0, 0, 0.2),
			2px 4px 16px 0px rgba(0, 0, 0, 0.2);
	}

	#service-img-chamber {
		/* width: 80vw; */
		height: 35vh;
		margin: 0 auto;
		border-radius: 8px;
		box-shadow:
			0px 1px 2px 0px rgba(0, 0, 0, 0.2),
			1px 2px 4px 0px rgba(0, 0, 0, 0.2),
			2px 4px 8px 0px rgba(0, 0, 0, 0.2),
			2px 4px 16px 0px rgba(0, 0, 0, 0.2);
	}

	/* No shadow */
	#brian-img {
		width: 400px;
		margin: 0 auto;
		border-radius: 8px;
	}

	#kw-logo-img {
		width: 320px;
		margin: 0 auto;
		border-radius: 8px;
	}

	.service-text {
		padding: 0 1rem;
		/* margin: 10px auto; */
	}

	/* SUBSCRIBE */

	.subscribe {
		text-align: center;
		display: flex;
		flex-direction: column;
	}
	.subscribe-social {
		display: flex;
		justify-content: center;
		gap: 3rem;
	}

	/* CONTACT */

	#contact {
		display: flex;
		flex-direction: column-reverse;
		gap: 3rem;
		margin: 3px 35px;
		/* margin-top: 3px; */
	}

	#calendly-icon {
		margin: 0 auto;
		width: 60px;
	}

	.cell-office-grid {
		display: grid;
		grid-template-columns: 1fr 1.7fr;
		gap: 0.25rem;
		width: 100%;
	}

	.cell-office-grid .mobile {
		justify-self: right;
	}
	.cell-office-grid .mobile-num {
		justify-self: left;
	}

	.contact-data {
		text-align: center;
	}

	/* @media screen and (min-width: 768) { */
	@media screen and (min-width: 576px) {
		nav {
			grid-template-columns: 1fr 2fr;
			gap: 2rem;
		}

		#hero-img {
			/* width: 100vw; */
			max-width: 470px;
		}

		#brian-img {
			width: 300px;
		}

		ul {
			padding-left: 32px;
			padding-right: 32px;
		}

		#service-img,
		#service-img-2 {
			width: 50vw;
		}

		#service-img-chamber {
			width: 45%;
			height: 90%;
			margin-top: 25px;
			margin-bottom: 50px;
		}

		.service-text {
			padding: 0 0rem;
		}

		#kw-logo-img {
			width: 400px;
		}

		.cell-office-grid {
			grid-template-columns: 1fr 1.35fr;
		}

		button {
			width: 50%;
			font-size: 1.75rem;
		}
	}

	@media screen and (min-width: 950px) {
		/* @media screen and (min-width: 900px) { */
		/* @media screen and (min-width: 768) { */
		/* .container {
			margin: 70px auto;
		} */

		nav {
			grid-template-columns: 1fr 2fr;
			gap: 2rem;
		}

		#hero-img {
			width: 70vw;
			max-width: 730px;
		}

		#brian-img {
			width: 300px;
		}

		ul {
			padding-left: 30px;
			padding-right: 30px;
			margin-bottom: 2px;
		}

		.services {
			margin: 20px;
		}

		button {
			width: 40%;
		}

		.row-1,
		.row-2 {
			display: grid;
			grid-template-columns: 1fr 1fr;
			gap: 2rem;
		}

		#service-img,
		#service-img-2 {
			width: 35vw;
			margin-top: 25px;
		}

		#service-img-chamber {
			width: 70%;
			height: 80%;
			margin-top: 25px;
		}

		.service-text p {
			/* padding: 0 1rem; */
			margin: 0px 30px;
		}

		#kw-logo-img {
			width: 300px;
			margin: 0 auto;
			border-radius: 8px;
		}

		.cell-office-grid {
			grid-template-columns: 1fr 1.2fr;
		}
	}

	/* ------------ */

	.nav-links a {
		font-size: 1.5rem;
		padding: 10px;
		text-decoration: none;
	}

	.nav-links a:hover {
		color: #2d3748;
	}
</style>
