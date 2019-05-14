<template>
	<div>
		<p>Counter is: {{doubleCounter}}</p>
		<hr>
		<p>Number of click: {{stringCounter}}</p>
	</div>
</template>

<script>
import { mapGetters } from "vuex";
export default {
	computed:{
		// counter() {
		// 	return this.$store.getters.doubleCounter;
		// },
		// clicks() {
		// 	return this.$store.getters.stringCounter;
		// }
        ...mapGetters(["doubleCounter", "stringCounter"]),
        

    }
};
</script>

<style>
</style>
