<script>
	export let slice;
	import { SliceSimulator } from '@slicemachine/adapter-sveltekit/simulator';

	/** @type {import("@prismicio/client").Content.ImageSlice} */

	console.log(slice);

	/** @type {import("@prismicio/client").Content.MemberslistSlice} */
</script>

<section>
	<img src={slice.primary.image.url} alt="" />

	<p>{slice.primary.name[0].text}</p>

	<ul>
		<li>Functie: Student</li>
		<li>leefttijd: 23 jaar</li>
		<li>Geboorteplaats: Amstelveen</li>
	</ul>

	Bezoek mijn<a href={slice.primary.link.url}>Github</a>!
</section>

<style>
	img {
		height: 100px;
		width: 100px;
	}
</style>
