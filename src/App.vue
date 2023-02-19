<script>
	export default {
	data() {
        return {
            attr: 'pip.png',
            name: 'маша',
            surname: 'фиалкова',
        }
    }
}
</script>
<template>
	<div>
        <img v-bind:src="attr">
		<p>{{ name }}</p>
    	<p>{{ surname }}</p>
	</div>
</template>
