<script>
	import ExcursionCard from './ExcursionCard.svelte';

	let excursions = [
		{
			name: 'Cocoa Beach Surf School',
			photo: {
				url: 'https://res.cloudinary.com/dinlug18r/image/upload/v1692936241/os2r6u83lvz2wmsfob0s.png',
				alt: 'Cocoa Beach Surf School'
			},
			description:
				'Learn to surf Solo surf lessons and group clinics located at the Historic Cocoa Beach Pier.'
		},
		{
			name: 'Cocoa Village',
			photo: {
				url: 'https://res.cloudinary.com/dinlug18r/image/upload/v1692936614/iaa6kozszfdndqrzb1r9.jpg',
				alt: 'Cocoa Village'
			},
			description:
				'Immerse yourself into Historic Cocoa Village. We give you our Map to the perfect historic adventure and with our wristband you can receive wine tastings, discounts at local shops, and much more.'
		},
		{
			name: 'Downtown Cocoa Beach',
			photo: {
				url: 'https://res.cloudinary.com/dinlug18r/image/upload/v1692937079/yrluxyidmvubskxe0oms.jpg',
				alt: 'Downtown Cocoa Beach'
			},
			description:
				'Check out the locals favorite restaurants and specialty shops. Get more out of your vacation with our helpful tour guide or take the reins yourself with our Map.  See all that beautiful Downtown Cocoa Beach has to offer.'
		},
		{
			name: 'Distillery and Brewery Tour',
			photo: {
				url: 'https://res.cloudinary.com/dinlug18r/image/upload/v1692937261/zcmcguay3f8puxot8rdt.png',
				alt: 'Distillery and Brewery Tour'
			},
			description:
				'First, stop by Oceanside Distillery for their Premium tour and tasting. Go behind the scenes and experience their handcrafted small batch process, hear from industry experts on distilling fresh from Florida spirits, enjoy your choice of neat or on the rocks spirit, or a hand-crafted cocktail at the tasting bar.'
		},
		{
			name: 'One Click Concierge',
			photo: {
				url: 'https://res.cloudinary.com/dinlug18r/image/upload/v1692937312/oru2zsrboiyvqt3rkor4.jpg',
				alt: 'One Click Concierge'
			},
			description:
				'Learn to surf Solo surf lessons and group clinics located at the Historic Cocoa Beach Pier.'
		},
		{
			name: 'Kayaking',
			photo: {
				url: 'https://res.cloudinary.com/dinlug18r/image/upload/v1692936511/drhdyfr3ouzdggqy21r5.webp',
				alt: 'Kayaking'
			},
			description:
				'Enjoy the Sunset tour or the nighttime Bioluminescence tour both located at Kiwanis Island Park, fun for the entire family, explore the river with a local and learn about our protected habitats.'
		}
	];
</script>

<div class="bg-gray-900 py-24 sm:py-32">
	<div class="mx-auto max-w-7xl px-6 lg:px-8">
		<div class="mx-auto max-w-2xl lg:mx-0">
			<h2 class="text-3xl font-bold tracking-tight text-white sm:text-4xl" id="excursions">
				Our Excursions
			</h2>
			<p class="mt-6 text-lg leading-8 text-gray-300">
				Blast off into the Florida Space Coast Culture.
			</p>
		</div>
		<ul
			role="list"
			class="mx-auto mt-20 grid max-w-2xl grid-cols-1 gap-x-8 gap-y-14 sm:grid-cols-2 lg:mx-0 lg:max-w-none lg:grid-cols-3 xl:grid-cols-4"
		>
			{#each excursions as excursion}
				<ExcursionCard {excursion} />
			{/each}

			<!-- More people... -->
		</ul>
	</div>
</div>
