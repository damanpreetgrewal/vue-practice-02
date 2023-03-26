<template>
	<select v-model="componentName">
		<option value="AppHome">Home</option>
		<option value="AppAbout">About</option>
	</select>
	<keep-alive>
		<component :is="componentName"></component>
	</keep-alive>
</template>

<script>
import AppHome from "./components/Home.vue";
import AppAbout from "./components/About.vue";
export default {
	name: "App",
	components: {
		AppHome,
		AppAbout,
	},
	data() {
		return {
			componentName: "AppHome",
		};
	},
};
</script>

<style>
#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
}
</style>
