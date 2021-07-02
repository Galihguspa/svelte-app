<script>
	//export let name;

	import NavigationBar from "./NavigationBar/NavigationBar.svelte";
	import Other from "./Other/Other.svelte";
	import { Col, Container, Row } from 'sveltestrap';

	let name = "Galih "
	let skill = ["Svelte","VueJS"]
	let ratingSkill = 80
	let imageURL = "image/svelte.png"
</script>
<NavigationBar/>
<Container>
	<main>
		<h2>Hello, <span class="nama"> {name}! </span> </h2>
		<hr>
		<p>Skill : <b>{skill}</b> </p>
		<p>Rating : <b>{ratingSkill}</b></p>
		<p>Jenis Kelamin : Laki Laki</p>
		
		<img src={imageURL} alt="Gambar Svelte" class="logo">

		<p>ini adalah dari css <span class="umum"> Global</span></p>
		<!---Other-->
		<Other/>

	</main>
</Container>

<style>
	.nama {
		color :red;
	}

	.logo{
		width : 50px
	}

</style>