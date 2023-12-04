<script setup>
import {ref} from 'vue'
let name = ref('')
let birth=ref(0)
let year=ref(0)

let names = ref(['илья','кирил','маша'])
let todos = ref([
    {status:false,name:'убраться дома'},



])

function addItem() {
    names.value.push({status: false, name: todo.value})
}
</script>


<template>
<div>

<input type="text" v-model="name" />

<button v-on:click.prevent="">добавить задание</button>

<p>Привет,{{ name}}</p>

<ul>
    <li v-for="name in names">{{ name }}</li>
</ul>

<ul>
    <li v-for="todo in todos"><input type="checkbox" v-model="todo.status"/>{{todo.name}}</li>
</ul>

</div>
</template>

<style scoped>

</style>
