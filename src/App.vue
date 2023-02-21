<script>
	export default {
	data() {
        return {
            attr: 'pip.png',
            name: 'маша',
            surname: 'фиалкова',
            var1: 5,
            var2: 2,
            arr2: [9, 10, 20],
            obj: { a: 3, b: 8, c: 9 },
        }
    },
   methods: {
        show: function () {
            alert(today);
        }
    }
}
let today = new Date();
</script>
<template>
	<div>
        <img v-bind:src="attr">
		<p>{{ name }}</p>
    	<p>{{ surname }}</p>
        {{ (var1**2) + var2 }}
        <br>{{ arr2[0] + arr2[1] + arr2[2] }}
    	<br>{{ obj.a + obj.b + obj.c }}
        <br><button class="button button1" @click="show">Узнать дату(нажатие)</button> <br> 
        <br><button class="button button2" @mouseenter="show"> Узнать дату(навестись)</button> 
	</div>
</template>
