<!--el script setup sirve para ahorrar trabajo ya que vue interpreta el codigo -->
<script setup>
import { ref } from 'vue'

let counter = ref(5);

function add(){
	counter.value++;
	console.log(counter);
	
}
</script>

<template>
	<div @click="add" class="font-semibold text-white select-none hover:cursor-pointer bg-blue-600 rounded py-1 px-2 max-w-44 text-center">
		Número de clicks: {{ counter }}
		</div>
</template>