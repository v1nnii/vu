<script>
	export default {
	data() {
        return {
            attr: 'pip.png',
            name: 'маша',
            surname: 'фиалкова',
            var1: 5,
            var2: 2,
        }
    }
}
</script>
<template>
	<div>
        <img v-bind:src="attr">
		<p>{{ name }}</p>
    	<p>{{ surname }}</p>
        {{ (var1**2) + var2 }}
	</div>
</template>
