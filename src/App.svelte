<script lang="ts">
	import Header from './Header.svelte'
	import USP from './USP.svelte';
	import Card from './Card.svelte';
	import Footer from './Footer.svelte';
</script>

<main>
	<Header></Header>
	<USP></USP>
	<Card></Card>
	<Footer></Footer>
</main>

<style>
main {
	display: flex;
	flex-direction: column;
	align-items: center;
}
</style>