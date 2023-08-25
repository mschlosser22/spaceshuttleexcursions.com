<script>
	export let excursion;
</script>

<li>
	<img class="aspect-[14/13] w-full rounded-2xl object-cover" src={excursion.photo.url} alt="" />
	<h3 class="mt-6 text-lg font-semibold leading-8 tracking-tight text-white">{excursion.name}</h3>
	<p class="text-sm leading-6 text-gray-500">{excursion.description}</p>
</li>
