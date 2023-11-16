<script>
	let showMobileMenu = false;
</script>

<div class="bg-gray-900 text-white">
	<header class="absolute inset-x-0 top-0 z-50">
		<nav
			class="mx-auto flex max-w-7xl items-center justify-between p-6 lg:px-8"
			aria-label="Global"
		>
			<div class="flex lg:flex-1">
				<a href="#" class="-m-1.5 p-1.5">
					<span class="sr-only">Space Shuttle Excursions</span>
					<svg
						xmlns="http://www.w3.org/2000/svg"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="1.5"
						stroke="currentColor"
						class="w-6 h-6"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							d="M15.59 14.37a6 6 0 01-5.84 7.38v-4.8m5.84-2.58a14.98 14.98 0 006.16-12.12A14.98 14.98 0 009.631 8.41m5.96 5.96a14.926 14.926 0 01-5.841 2.58m-.119-8.54a6 6 0 00-7.381 5.84h4.8m2.581-5.84a14.927 14.927 0 00-2.58 5.84m2.699 2.7c-.103.021-.207.041-.311.06a15.09 15.09 0 01-2.448-2.448 14.9 14.9 0 01.06-.312m-2.24 2.39a4.493 4.493 0 00-1.757 4.306 4.493 4.493 0 004.306-1.758M16.5 9a1.5 1.5 0 11-3 0 1.5 1.5 0 013 0z"
						/>
					</svg>
				</a>
			</div>
			<div class="flex lg:hidden">
				<button
					type="button"
					class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-50"
					on:click={() => (showMobileMenu = true)}
				>
					<span class="sr-only">Open main menu</span>
					<svg
						class="h-6 w-6"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="1.5"
						stroke="currentColor"
						aria-hidden="true"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
						/>
					</svg>
				</button>
			</div>
			<div class="hidden lg:flex lg:gap-x-12">
				<a href="#" class="text-sm font-semibold leading-6 text-white">About</a>
				<a href="#excursions" class="text-sm font-semibold leading-6 text-white">Excursions</a>
				<a
					href="https://fareharbor.com/embeds/book/cocoabeachsurfschool/?full-items=yes&flow=492386"
					class="text-sm font-semibold leading-6 text-white">Book</a
				>
				<a href="#" class="text-sm font-semibold leading-6 text-white">Contact</a>
			</div>
			<div class="hidden lg:flex lg:flex-1 lg:justify-end">
				<a href="#" class="text-sm font-semibold leading-6 text-white"
					>Log in <span aria-hidden="true">&rarr;</span></a
				>
			</div>
		</nav>
		{#if showMobileMenu}
			<!-- Mobile menu, show/hide based on menu open state. -->
			<div class="lg:hidden" role="dialog" aria-modal="true">
				<!-- Background backdrop, show/hide based on slide-over state. -->
				<div class="fixed inset-0 z-50" />
				<div
					class="fixed inset-y-0 right-0 z-50 w-full overflow-y-auto bg-gray-900 px-6 py-6 sm:max-w-sm sm:ring-1 sm:ring-white/10"
				>
					<div class="flex items-center justify-between" id="about">
						<a href="#" class="-m-1.5 p-1.5">
							<span class="sr-only">Space Shuttle Excursions</span>
							<img
								class="h-8 w-auto"
								src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=600"
								alt=""
							/>
						</a>
						<button
							type="button"
							class="-m-2.5 rounded-md p-2.5 text-gray-50"
							on:click={() => (showMobileMenu = false)}
						>
							<span class="sr-only">Close menu</span>
							<svg
								class="h-6 w-6"
								fill="none"
								viewBox="0 0 24 24"
								stroke-width="1.5"
								stroke="currentColor"
								aria-hidden="true"
							>
								<path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
							</svg>
						</button>
					</div>
					<div class="mt-6 flow-root">
						<div class="-my-6 divide-y divide-black-500/10">
							<div class="space-y-2 py-6">
								<a
									href="#excursions"
									on:click={() => (showMobileMenu = false)}
									class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-white hover:bg-gray-50"
									>Excursions</a
								>
								<a
									href="https://fareharbor.com/embeds/book/cocoabeachsurfschool/?full-items=yes&flow=492386"
									on:click={() => (showMobileMenu = false)}
									class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-white hover:bg-gray-50"
									>Book</a
								>
								<a
									href="#about"
									on:click={() => (showMobileMenu = false)}
									class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-white hover:bg-gray-50"
									>About</a
								>
								<a
									href="#"
									on:click={() => (showMobileMenu = false)}
									class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-white hover:bg-gray-50"
									>Contact</a
								>
							</div>
						</div>
					</div>
				</div>
			</div>
		{/if}
	</header>
	<main>
		<div class="relative isolate">
			<svg
				class="absolute inset-x-0 top-0 -z-10 h-[64rem] w-full stroke-gray-800 [mask-image:radial-gradient(32rem_32rem_at_center,white,transparent)]"
				aria-hidden="true"
			>
				<defs>
					<pattern
						id="1f932ae7-37de-4c0a-a8b0-a6e3b4d44b84"
						width="200"
						height="200"
						x="50%"
						y="-1"
						patternUnits="userSpaceOnUse"
					>
						<path d="M.5 200V.5H200" fill="none" />
					</pattern>
				</defs>
				<svg x="50%" y="-1" class="overflow-visible fill-black-100">
					<path
						d="M-200 0h201v201h-201Z M600 0h201v201h-201Z M-400 600h201v201h-201Z M200 800h201v201h-201Z"
						stroke-width="0"
					/>
				</svg>
				<rect
					width="100%"
					height="100%"
					stroke-width="0"
					fill="url(#1f932ae7-37de-4c0a-a8b0-a6e3b4d44b84)"
				/>
			</svg>
			<div
				class="absolute left-1/2 right-0 top-0 -z-10 -ml-24 transform-gpu overflow-hidden blur-3xl lg:ml-24 xl:ml-48"
				aria-hidden="true"
			>
				<div
					class="aspect-[801/1036] w-[50.0625rem] bg-gradient-to-tr from-[#ff80b5] to-[#9089fc] opacity-30"
					style="clip-path: polygon(63.1% 29.5%, 100% 17.1%, 76.6% 3%, 48.4% 0%, 44.6% 4.7%, 54.5% 25.3%, 59.8% 49%, 55.2% 57.8%, 44.4% 57.2%, 27.8% 47.9%, 35.1% 81.5%, 0% 97.7%, 39.2% 100%, 35.2% 81.4%, 97.2% 52.8%, 63.1% 29.5%)"
				/>
			</div>
			<div class="overflow-hidden">
				<div class="mx-auto max-w-7xl px-6 pb-32 pt-36 sm:pt-60 lg:px-8 lg:pt-32">
					<div class="mx-auto max-w-2xl gap-x-14 lg:mx-0 lg:flex lg:max-w-none lg:items-center">
						<div class="w-full max-w-xl lg:shrink-0 xl:max-w-2xl">
							<h1 class="text-4xl font-bold tracking-tight text-white sm:text-6xl">
								Space Shuttle Excursions
							</h1>
							<p class="relative mt-6 text-lg leading-8 text-gray-200 sm:max-w-md lg:max-w-none">
								Space Shuttle is an exciting excursion company that offers a range of unique
								experiences for adventure enthusiasts. With Space Shuttle, you can indulge in
								unforgettable experiences that cater to diverse interests and create lasting
								memories.
							</p>
							<div class="mt-10 flex items-center gap-x-6">
								<a
									href="https://fareharbor.com/embeds/book/cocoabeachsurfschool/?full-items=yes&flow=492386"
									class="rounded-md bg-indigo-600 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
									>Book Now</a
								>
								<a href="#" class="text-sm font-semibold leading-6 text-white"
									>Contact Us <span aria-hidden="true">→</span></a
								>
							</div>
						</div>
						<div
							class="mt-14 flex justify-end gap-8 sm:-mt-44 sm:justify-start sm:pl-20 lg:mt-0 lg:pl-0"
						>
							<div
								class="ml-auto w-44 flex-none space-y-8 pt-32 sm:ml-0 sm:pt-80 lg:order-last lg:pt-36 xl:order-none xl:pt-80"
							>
								<div class="relative">
									<img
										src="https://res.cloudinary.com/dinlug18r/image/upload/v1692933818/tencsfkidwybsbz1nyho.jpg"
										alt=""
										class="aspect-[2/3] w-full rounded-xl bg-gray/5 object-cover shadow-lg"
									/>
									<div
										class="pointer-events-none absolute inset-0 rounded-xl ring-1 ring-inset ring-white/10"
									/>
								</div>
							</div>
							<div class="mr-auto w-44 flex-none space-y-8 sm:mr-0 sm:pt-52 lg:pt-36">
								<div class="relative">
									<img
										src="https://res.cloudinary.com/dinlug18r/image/upload/t_cocoa-village-crop/2689401_Cocoa_DSC4846-copy-2000-fd30f1647c7548139edd90cb48550757_aarsie.jpg"
										alt=""
										class="aspect-[2/3] w-full rounded-xl bg-white/5 object-cover shadow-lg"
									/>
									<div
										class="pointer-events-none absolute inset-0 rounded-xl ring-1 ring-inset ring-white/10"
									/>
								</div>
								<div class="relative">
									<img
										src="https://res.cloudinary.com/dinlug18r/image/upload/v1692934305/wza3hmdpzvwv9vdi9tki.jpg"
										alt=""
										class="aspect-[2/3] w-full rounded-xl bg-white/5 object-cover shadow-lg"
									/>
									<div
										class="pointer-events-none absolute inset-0 rounded-xl ring-1 ring-inset ring-white/10"
									/>
								</div>
							</div>
							<div class="w-44 flex-none space-y-8 pt-32 sm:pt-0">
								<div class="relative">
									<img
										src="https://res.cloudinary.com/dinlug18r/image/upload/v1692935124/vfsnbln7t8wfxuieisk9.jpg"
										alt=""
										class="aspect-[2/3] w-full rounded-xl bg-white/5 object-cover shadow-lg"
									/>
									<div
										class="pointer-events-none absolute inset-0 rounded-xl ring-1 ring-inset ring-white/10"
									/>
								</div>
								<div class="relative">
									<img
										src="https://res.cloudinary.com/dinlug18r/image/upload/v1692935790/aua71igdksuavgjw2roq.jpg"
										alt=""
										class="aspect-[2/3] w-full rounded-xl bg-white/5 object-cover shadow-lg"
									/>
									<div
										class="pointer-events-none absolute inset-0 rounded-xl ring-1 ring-inset ring-white/10"
									/>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</main>
</div>
