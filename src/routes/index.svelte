<script>
	import { Router, Route } from "svelte-routing";
	import Home from "../components/Home.svelte";
	import Item from "../components/Item.svelte";


	export let url = "/";
</script>

<Router {url}>
	<Route path="/" component={Home} />
	<Route path="item" component={Item} />
</Router>