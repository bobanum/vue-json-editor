<template>
	<div id="app">
		<header><h1>Header</h1></header>
		<main-nav><li><a href="#">Extra</a></li></main-nav>
		<div class="body">Contents</div>
		<footer>Footer</footer>
	</div>
</template>

<script>
import MainNav from "./components/MainNav";
export default {
	name: 'App',
	components: {
		MainNav,
	}
}
</script>

<style lang="scss">
:root {
	--hue: 30;
	--sat: 60%;
}
html {
	height: 100%;
}
body {
	height: 100%;
	margin: 0;
	background-color: hsl(var(--hue), var(--sat), 20%);
	color: hsl(var(--hue), var(--sat), 95%);
}
#app {
	min-height: 100%;
	display: flex;
	flex-direction: column;
	font-family: Avenir, Helvetica, Arial, sans-serif;
	& > * {
		padding: .5em 1em;
	}
	& > header {
		background-color: hsl(var(--hue), var(--sat), 15%);
	}
	& > nav {
		background-color: hsl(var(--hue), var(--sat), 10%);
	}
	& > .body {
		flex: 1 0 auto;
	}
	& > footer {
		background-color: hsl(var(--hue), var(--sat), 10%);
	}
}

</style>
