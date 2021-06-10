<template>
    <div class="p-4" style="background-color:aliceblue">
        <h1 class="mb-6 text-xl">Tugas Vue 4</h1>
        <ul>
            <li v-for="user in users"
                v-bind:key="user.id"
                class="w-1/4 mx-auto border-2 border-blue-300 m-4 p-2 text-gray-600 uppercase text-sm 
                rounded-lg shadow-md font-semibold bg-blue-200"
            >
            <router-link :to="{name:'User-Detail',params:{user: user}}">{{ user.name }} </router-link></li>
        </ul>
    </div>   
</template>

<script>

    export default {
        data() {
            return {
                users: []
            }
        },
        mounted() {
            axios
            .get("https://jsonplaceholder.typicode.com/users")
            .then((response) => (this.users = response.data))
        }
    }

</script>

<style scoped>

</style>
