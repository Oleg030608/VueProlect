<script setup>

const todos = [
    { userId: 1, id: 1, title: "Купить еды", completed: false },
    { userId: 2, id: 2, title: "Сделать дз", completed: false },
]

</script>

<template>
    <ul>
        <li v-for="todo in todos" v-bind:key="todo.id">
        <input type="checkbox" v-model="todo.completed">{{ todo.title }}({{ todo.userId }})❌
        </li>
    </ul>


</template>

<style scoped>
ul {
    margin-top: 0 auto;
    width: 500px;
    list-style: none;
}
</style>
