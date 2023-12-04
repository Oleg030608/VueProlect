<script setup>
import { ref } from "vue";
const users = ref([  
 { id: 1, username: 'ОЛег'},
 { id: 2, username: 'Дима'},
 { id: 3, username: 'Макс'}
])

</script>

<template>
    <form>
        <select>
            <option value="value1">олег</option>
        </select>
        <!-- <button>Добавить</button> -->


        <input type="text" v-model="name" />
        <button v-on:click.prevent="">new todo</button>
        <input type="text" v-model="name" class="users-input"/>
        <button v-on:click.prevent="">select user</button>
    </form>
</template>    

<style scoped>
form {
    display: flex;
    flex-direction: column;
}


</style>
