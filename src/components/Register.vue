<script setup>
</script>

<template>
    <div class="todo-form">
        <input type="text" v-model="name" />
        <button v-on:click.prevent="">new todo</button>
        <input type="text" v-model="name" class="users-input"/>
        <button v-on:click.prevent="">select user</button>
    </div>
</template>

<style scored>
.todo-form {
    width: 50%;
    display: flex;
    flex-direction: column;
}
.users-input{
    margin-top: 25px;
}

</style>