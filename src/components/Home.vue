<template>
	<p>Home</p>
</template>

<script>
export default {
	name: "AppHome",
	unmounted() {
		console.log("Home component unmounted");
	},
	mounted() {
		console.log("Home component mounted");
	},
	activated() {
		console.log("Home component activated");
	},
	deactivated() {
		console.log("Home component deactivated");
	},
};
</script>
