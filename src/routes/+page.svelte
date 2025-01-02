<script>
	let clientEmail = $state('');
	let clientFirst = $state('');
	let clientLast = $state('');

	let menuOpen = $state(false);

	function toggleMenu() {
		menuOpen = !menuOpen;
	}
</script>

<nav class="mb-10 bg-gray-100 fixed top-0 left-0 right-0 z-50">
	<a href="/" title="My Guy Bri HOME">
		<img class="py-1" id="my-guy-bri-img" src="my-guy-bri-logo.jpg" alt="hero kitchen" />
	</a>
	<div class="nav-links text-gray-500 hidden md:flex">
		<a href="#about-me" title="About Brian">About Brian</a>
		<a href="#search-homes" title="Search properties">Search</a>
		<a href="#our-services" title="My services">Services</a>
		<a href="#contact-me" title="Contact Brian">Contact</a>
	</div>
	<div class="md:hidden">
		<button onclick={toggleMenu} class="hamburger">
			{#if menuOpen}
				<span>&#x2715;</span> <!-- X icon -->
			{:else}
				<span>&#9776;</span> <!-- Hamburger icon -->
			{/if}
		</button>
	</div>
</nav>

{#if menuOpen}
	<div class="mobile-menu bg-gray-100 text-gray-500">
		<a href="#about-me" title="About Brian" onclick={toggleMenu}>About Brian</a>
		<a href="#search-homes" title="Search properties" onclick={toggleMenu}>Search</a>
		<a href="#our-services" title="My services" onclick={toggleMenu}>Services</a>
		<a href="#contact-me" title="Contact Brian" onclick={toggleMenu}>Contact</a>
	</div>
{/if}

<div class="container">
	<section>
		<div class="hero-image pt-2 mb-4">
			<img id="hero-img" src="pexels-frans-van-heerden-201846-1438834.jpg" alt="hero kitchen" />
		</div>

		<p class="mx-10 md:mx-24 lg:mx-44 text-xl text-gray-500">
			Are you looking for a real estate <span style="color: #334070;">professional</span> who will put your needs first?
		</p>

		<p class="mx-10 md:mx-24 lg:mx-44 text-xl text-gray-500">
			Are you looking for an
			<span style="color: #334070;">expert</span> who has extensive knowledge of the Greater Orlando
			market?
		</p>

		<p class="mx-10 md:mx-24 lg:mx-44 text-xl text-gray-500">
			Are you looking for a <span style="color: #334070;">partner</span> to provide you valuable insight
			so that you can make the best decisions until the completion of your buying or selling process?
		</p>

		<p class="mx-10 md:mx-24 lg:mx-44 text-xl text-gray-500">
			<em>Congratulations!</em> You've found <span style="color: #334070;">Brian Altomari</span>,
			and your search has come to a close.
		</p>

		<div class="service-image mt-4">
			<img id="kw-logo-img" src="ba-kw-logo-larger-crop.jpg" alt="hero kw" />
		</div>

		<div id="search-homes" class="mb-0"></div>

		<div class="hero-text text-center">
			<h2 class=" text-3xl text-red-500 pb-2">Let Me Help You</h2>
			<h2 class=" text-3xl text-red-500">Find Your Florida Dream Home</h2>
		</div>

		<div class="hero-btn">
			<form action="https://brianaltomari.kw.com" target="_blank">
				<!-- <button type="submit">Search For Yo/ur New Home Now</button> -->
				<button type="submit">Dream Home Search</button>
			</form>
		</div>

		<p class="mx-10 mb-0 font-semibold text-2xl text-blue-800"><em>I'm glad you stopped by!</em></p>
		<p class="mx-10 md:mx-24 lg:mx-44 text-xl text-gray-500">
			There's so much to see here, so take your time, look around, and learn all there is to know
			about us. We hope you enjoy our site and take a moment to drop us a line.
		</p>
	</section>

	<div id="about-me" class="mb-12"></div>

	<div class="my-hr">
		<hr class="hr-1" />
		<h4 class="middle-text">Meet Brian</h4>
		<hr class="hr-2" />
	</div>

	<!-- see: https://www.sitepoint.com/style-html-details-element/ -->
	<div class="about-brian">
		<img id="brian-img" src="brian-image-crop.jpg" alt="Brian Altomari" />
		<p class="pt-2 mb-0 px-3 text-center leading-8 text-gray-500">License #: SL3619639</p>
		<p class="pt-3 mb-4 px-3 md:text-xl lg:mx-28 text-justify leading-8 text-gray-500">
			<!-- <p class="mx-8 mb-2 px-3 text-justify leading-8 text-gray-500"> -->
			It's key that you get to know who I am as a person, and why I'm the best REALTOR® to help you
			with such an important transaction which is deeply personal to YOU.
		</p>
		<ul class="pt-3 mb-4 px-3 md:text-xl lg:mx-28 text-justify leading-8 text-gray-500">
			<li>This is <em>not</em> a side hustle.</li>
			<li>This is <em>not</em> something I'm doing because it looked cool on TV.</li>
			<!-- <li>
				This has <em>nothing</em> to do with Phil Dunphy (though I am a fan of <em>Modern Family</em>).
			</li> -->
			<li>This is my passion; it's my full-time career.</li>
			<!-- <li class="mt-3 text-center">
				<span class="text-xl text-blue-800 font-bold"
					>I'M ALL IN FOR <em class="text-2xl">YOU</em></span
				>.
			</li> -->
		</ul>
		<p class="mb-3 px-3 md:text-xl lg:mx-28 text-justify leading-8 text-gray-500">
			I know both sides of real estate in Florida, and my personal commitment is to make your life
			easier. I'll make this process professional and FUN! 🎈
		</p>
		<p class="mb-4 px-3 text-center">
			<span class="text-xl text-blue-800 font-bold"
				>I'm Brian, and I'm ALL IN FOR <em class="text-2xl">YOU!</em></span
			>
		</p>
		<div class="signature flex flex-row justify-end">
			<img id="brian-signature" src="brian-signature-crop.png" alt="signature" />
		</div>
		<details close style="cursor: pointer; margin-top: 1.5rem;">
			<summary><em> More about Brian...</em></summary>
			<p class="mb-4 mt-2 px-3 md:text-xl lg:mx-28 text-justify leading-8 text-gray-500">
				My organizational skills are unmatched, and I live by the <a
					class="font-underline text-sky-500 hover:text-sky-700"
					href="https://www.forbes.com/councils/forbescoachescouncil/2020/03/10/mamba-mentality-the-mindset-it-takes-to-be-the-best/"
					target="_blank"
					>Mamba Mentality
				</a>, so you are going to get the absolute best that I have to offer in every step of your
				transaction each and every day.
			</p>
			<p class="mb-4 px-3 md:text-xl lg:mx-28 text-justify leading-8 text-gray-500">
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Officia atque quis est quam
				perferendis! Nesciunt ipsa fugiat ut consectetur explicabo dolores possimus dolor minima
				molestiae nulla, consequuntur provident eligendi fugit?
			</p>
		</details>
	</div>

	<div id="our-services" class="mb-12"></div>

	<div class="my-hr">
		<hr class="hr-1" />
		<h4 class="middle-text">Our Services</h4>
		<hr class="hr-2" />
	</div>

	<div class="services">
		<div class="row-1">
			<div class="service-image">
				<img id="service-img" src="naomi-hebert-MP0bgaS_d1c-unsplash.jpg" alt="hero kitchen" />
			</div>
			<div class="service-text">
				<h2 class="mx-8 py-4 text-3xl text-blue-800">Real Estate Done <em>Right</em></h2>
				<p class="mx-8 mb-2 px-3 md:text-xl md:mx-20 text-justify leading-8 text-gray-500">
					Nervous about your property adventure? Don’t be. Whether you're getting ready to buy or
					sell, in the middle of it, or just looking for some answers, our top-notch skills ensure
					you get the best experience possible. It’s what we love to do.
				</p>
			</div>
		</div>

		<div class="row-2">
			<div class="service-text">
				<h2 class="mx-8 py-4 text-3xl text-blue-800">Rely on Expertise</h2>
				<p
					class="mx-8 mb-2 px-3 md:text-xl md:mx-20 lg:text-xl text-justify leading-8 text-gray-500"
				>
					If you have questions about and and all things real estate, trust us to find you what you
					need fast. We make sure you feel confident and educated every step of the way. We pride
					ourselves in being your trusted residential real estate resource.
				</p>
			</div>
			<div class="service-image">
				<img id="service-img-2" src="pexels-mikhail-nilov-9400877.jpg" alt="hero kitchen" />
			</div>
		</div>

		<div class="row-1">
			<div class="service-image">
				<img id="service-img" src="kw-outside-crop.jpg" alt="hero kw" />
			</div>
			<div class="service-text">
				<!-- <h2 class="mx-8 py-4 text-3xl text-blue-800">Rely on KW</h2> -->
				<div class="service-image mt-4 pb-4">
					<img id="kw-logo-img" src="ba-kw-logo-larger-crop.jpg" alt="hero kw" />
				</div>
				<p
					class="mx-8 mb-2 px-3 md:text-xl md:mx-20 lg:text-xl text-justify leading-8 text-gray-500"
				>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore autem, mollitia aliquam
					dolorem corrupti id voluptatibus enim quas tempora nulla, corporis ea repellendus
					veritatis ut provident at, est excepturi optio?
				</p>
				<p
					class="mx-8 mb-2 px-3 md:text-xl md:mx-20 lg:text-xl text-justify leading-8 text-gray-500"
				>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore autem, mollitia aliquam
					dolorem corrupti id voluptatibus enim quas tempora nulla, corporis ea repellendus
					veritatis ut provident at, est excepturi optio?
				</p>
			</div>
		</div>
	</div>

	<!-- <h1>Subscribe</h1>
	
	<p class="mb-2 text-gray-500">Sign up for real estate news.</p>
	
		<section>
			<div class="sm:col-span-4">
				<label for="email" class="block text-sm/6 font-medium text-gray-900">Email address</label>
				<div class="mt-2">
					<input
					id="email"
					name="email"
					type="email"
					bind:value={clientEmail}
					autocomplete="email"
					class="block w-full rounded-md bg-white px-3 py-1.5 text-base text-gray-900 outline outline-1 -outline-offset-1 outline-gray-300 placeholder:text-gray-400 focus:outline focus:outline-2 focus:-outline-offset-2 focus:outline-indigo-600 sm:text-sm/6"
					/>
					</div>
					</div>
			</section> -->

	<div id="contact-me" class="mb-12"></div>

	<div class="my-hr">
		<hr class="hr-1" />
		<h4 class="middle-text">Call or Visit</h4>
		<hr class="hr-2" />
	</div>

	<!-- <img id="winter-park-img" src="winter-park-wide.jpg" alt="winter park" /> -->

	<div id="contact">
		<div class="contact-form">
			<form>
				<div class="space-y-12">
					<!-- <div class="border-b border-gray-900/10 pb-2"> -->
					<div>
						<h2 class="text-2xl font-semibold text-blue-900">Contact Brian</h2>

						<div class="mt-4 grid grid-cols-1 gap-x-6 gap-y-2 sm:grid-cols-6">
							<div class="sm:col-span-3">
								<label for="first-name" class="block text-sm/6 font-medium text-gray-900"
									>First name</label
								>
								<div class="mt-2">
									<input
										type="text"
										name="first-name"
										id="first-name"
										autocomplete="given-name"
										class="w-full rounded-md bg-white px-3 py-1.5 text-base text-gray-900 outline outline-1 -outline-offset-1 outline-gray-300 placeholder:text-gray-400 focus:outline focus:outline-2 focus:-outline-offset-2 focus:outline-indigo-600 sm:text-sm/6"
									/>
								</div>
							</div>

							<div class="sm:col-span-3">
								<label for="last-name" class="block text-sm/6 font-medium text-gray-900"
									>Last name</label
								>
								<div class="mt-2">
									<input
										type="text"
										name="last-name"
										id="last-name"
										autocomplete="family-name"
										class="block w-full rounded-md bg-white px-3 py-1.5 text-base text-gray-900 outline outline-1 -outline-offset-1 outline-gray-300 placeholder:text-gray-400 focus:outline focus:outline-2 focus:-outline-offset-2 focus:outline-indigo-600 sm:text-sm/6"
									/>
								</div>
							</div>

							<div class="sm:col-span-4">
								<label for="email" class="block text-sm/6 font-medium text-gray-900"
									>Email address</label
								>
								<div class="mt-2">
									<input
										id="email"
										name="email"
										type="email"
										bind:value={clientEmail}
										autocomplete="email"
										class="block w-full rounded-md bg-white px-3 py-1.5 text-base text-gray-900 outline outline-1 -outline-offset-1 outline-gray-300 placeholder:text-gray-400 focus:outline focus:outline-2 focus:-outline-offset-2 focus:outline-indigo-600 sm:text-sm/6"
									/>
								</div>
							</div>
						</div>
					</div>
				</div>

				<div class="col-span-full">
					<label for="about" class="mt-3 block text-sm/6 font-medium text-gray-900"
						><em>How can I help?</em></label
					>
					<p class="mt-0 text-sm/6 text-gray-500">
						<!-- <em>Please write a few sentences about what you're looking for.</em> -->
					</p>
					<div class="mt-2">
						<textarea
							name="about"
							id="about"
							rows="3"
							placeholder="Please write a few sentences about what you're looking for..."
							class="block w-full rounded-md bg-white px-3 py-1.5 text-base text-gray-900 outline outline-1 -outline-offset-1 outline-gray-300 placeholder:text-blue-400 focus:outline focus:outline-2 focus:-outline-offset-2 focus:outline-indigo-600 sm:text-sm/6"
						>
						</textarea>
					</div>
				</div>

				<div class="mb-8 mt-4 flex">
					<!-- Interested? Let's Talk! -->
					<!-- <button type="button" class="text-sm/6 font-semibold text-gray-900">Cancel</button> -->
					<button type="submit" style="flex: 110;" class="text-sm font-semibold text-gray-900"
						>Send</button
					>
				</div>
			</form>
		</div>

		<div id="contact-me" class="contact-data">
			<h2 class="mb-4 text-4xl font-semibold text-blue-900">Brian Altomari</h2>
			<h2 class="text-xl" id="mobile">Mobile: (312) 420-3587</h2>
			<h4 class="text-xl mb-4" id="office">Office: (407) 545-6430</h4>
			<h4 class="text-xl mb-6" id="bri-email">
				<a
					class="text-2xl text-blue-500 border-gray-300 hover:text-orange-500"
					outline
					color="dark"
					href="mailto: brianaltomari@kw.com?subject=My Guy Bri ({clientFirst} {clientLast}) Inquiry"
					target="_blank"
					rel="noopener noreferrer">brianaltomari@kw.com</a
				>
			</h4>

			<div class="subscribe mb-12">
				<div class="subscribe-social mt-0">
					<a
						href="https://www.facebook.com/people/Brian-Altomari-Orlando-Realtor/61565822827296/"
						target="_blank"
						style="cursor: pointer;"
						title="Brian's Facebook Page"
					>
						<img src="facebook_2504903.png" alt="facebook icon" />
					</a>
					<a
						href="https://www.instagram.com/brianaltomari_realtor/"
						target="_blank"
						style="cursor: pointer;"
						title="Brian on Instagram"
					>
						<img src="instagram_2111463.png" alt="instagram icon" />
					</a>
					<a
						href="https://www.linkedin.com/in/brian-altomari-5a719961/"
						target="_blank"
						style="cursor: pointer;"
						title="Brian's LinkedIn Profile"
					>
						<img src="linkedin_2504923.png" alt="instagram icon" />
					</a>
					<a
						href="https://www.youtube.com/@brianaltomari_realtor"
						target="_blank"
						style="cursor: pointer;"
						title="Brian's YouTube Channel"
					>
						<img src="youtube_4096116.png" alt="instagram icon" />
					</a>
				</div>
			</div>

			<div style="margin: 2rem auto 0 auto;">
				<!-- <img id="kw-logo-img" src="ba-kw-logo-larger.jpg" alt="hero kw" /> -->
				<img id="kw-logo-img" src="my-guy-bri-kw-logo.jpg" alt="hero kw" />
			</div>
			<!-- <h4 id="address-1" class="mb-1 font-semibold text-slate-900">Keller Williams Winter Park</h4> -->
			<h4 class="text-2xl mt-3 font-semibold" id="address-0">Keller Williams Realty</h4>
			<h4 class="text-xl mt-2" id="address-2">147 W. Lyman Avenue</h4>
			<h4 class="text-xl" id="address-3">Winter Park, FL 32789</h4>
		</div>
	</div>
</div>

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
		font-size: 1rem;
		display: flex;
		gap: 0.8rem;
	}

	.nav-links a:hover {
		color: orangered;
		cursor: pointer;
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
		width: 12rem;
		/* border: 1px solid orangered;
		color: orangered; */
		border: 1px solid #041e42;
		color: #041e42;
		opacity: 0.75;
		font-size: 1.25rem;
		margin-bottom: 15px;
	}
	button:hover {
		background-color: #041e42;
		color: #fff;
		opacity: 1;
	}

	.my-hr {
		display: flex;
		align-items: center;
		margin-top: 30px;
	}

	.hr-1,
	.hr-2 {
		border: 1px lightgray solid;
		margin: 20px;
		flex: 1 1 0;
	}

	/* ABOUT */
	.about-brian {
		margin: 0 auto;
		width: 80%;
	}

	/* summary {
		list-style-position: outside;
		margin-left: 30px;
		padding: 10px 10px 10px 20px;
		border-radius: 5px;
		list-style-type: '⬇ ';
		color: #334070;
	} */
	summary {
		display: flex;
		align-items: center;
		color: #334070;
	}

	summary::after {
		content: '';
		width: 18px;
		height: 10px;
		/* background: url('arrow.svg'); */
		background: url('https://uploads.sitepoint.com/wp-content/uploads/2023/10/1697699669arrow.svg')
			no-repeat;
		background-size: cover;
		margin-left: 0.75em;
		transition: 0.2s;
	}

	details[open] > summary::after {
		transform: rotate(180deg);
	}

	/* sigh, Safari again */

	summary::-webkit-details-marker {
		display: none;
	}

	summary::marker {
		color: orangered;
		font-size: 1.2em;
	}

	/* details[open] > summary {
		list-style-type: '⬆ ';
	} */

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

	/* No shadow */
	#brian-img,
	#kw-logo-img {
		width: 400px;
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
	.subscribe h1 {
		font-size: 2.5rem;
		color: orangered;
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
		margin: 35px;
	}

	.contact-form {
		/* flex: 110; */
		margin: 0 auto;
	}

	.contact-data {
		text-align: center;
		/* flex: 110; */
		/* padding-left: 1rem; */
	}

	/* #mobile,
	#office,
	#bri-email,
	#address-1,
	#address-2,
	#address-3 { */
	/* padding-left: 1rem; */
	/* } */

	#winter-park-img {
		/* width: 600px; */
		margin: 0px auto;
		border-radius: 8px;
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

		#service-img,
		#service-img-2 {
			width: 50vw;
		}

		.service-text {
			padding: 0 0rem;
		}

		#kw-logo-img {
			width: 300px;
			margin: 0 auto;
			border-radius: 8px;
		}
	}

	@media screen and (min-width: 900px) {
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

		.services {
			margin: 20px;
		}

		/* .row-1,
		.row-2 {
			flex-direction: row;
			align-items: center;
		} */

		/* .row-2 {
			flex-direction: row;
		} */

		.row-1,
		.row-2 {
			display: grid;
			grid-template-columns: 1fr 1fr;
			gap: 2rem;
		}

		#service-img,
		#service-img-2 {
			width: 35vw;
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
	}

	/* ------------ */
	/* ------------ */
	/* ------------ */

	.hamburger {
		font-size: 24px;
		background: none;
		border: none;
		cursor: pointer;
	}

	.mobile-menu {
		display: flex;
		flex-direction: column;
		position: absolute;
		top: 60px;
		left: 0;
		right: 0;
		/* background-color: #f7fafc; bg-gray-100 */
		padding: 1rem;
	}

	.mobile-menu a {
		padding: 10px;
		border-bottom: 1px solid #ccc;
		text-align: center;
		width: 100%;
	}

	.nav-links a {
		padding: 10px;
		text-decoration: none;
		color: #4a5568;
	}

	.nav-links a:hover {
		color: #2d3748;
	}
</style>
