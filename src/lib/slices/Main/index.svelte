<script>
    export let slice;
import { SliceSimulator } from "@slicemachine/adapter-sveltekit/simulator";

/** @type {import("@prismicio/client").Content.ImageSlice} */


console.log(slice)
</script>
<section data-slice-type={slice.slice_type} data-slice-variation={slice.variation}>



<img src={slice.primary.image.url} alt="">

<p>{slice.primary.name[0].text}</p>

<ul>
    <li>
        Functie: Student
    </li>
    <li>
        leefttijd: 23 jaar
    </li>
    <li>
        Geboorteplaats: Amstelveen
    </li>
</ul>

Bezoek mijn <a href={slice.primary.link.url}>Github</a>!

</section>

<style>

img{
height: 100px;
width: 100px;
}

</style>