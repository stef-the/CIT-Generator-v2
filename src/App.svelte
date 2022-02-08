<script>
	import router from "page";
	import Home from "./components/Home.svelte";
	import Item from "./components/Item.svelte";

	let page;

	router("/", () => (page = Home));
	router("/item", () => (page = Item));

	router.start();
</script>
<svelte:component this={page} />