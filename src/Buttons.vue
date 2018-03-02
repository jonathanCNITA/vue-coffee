<template>
	<div>
		<div class="all-buttons" v-for="machine in machines">
      		<label for="bt">MASCHINE {{ machine.id }}</label>
      		<toggle-button name="bt" :sync="true" v-model="machine.state"/>
    	</div>
	</div>
</template>

<script>
	export default {
		data() {
			return {
				machines: [
			        {id: 1, state: true},
			        {id: 2, state: false},
			        {id: 3, state: true},
			        {id: 4, state: false},
			        {id: 5, state: false},
			        {id: 6, state: false}
			      ]
			}
		}
	}
</script>