<template>
    <div class="pb-48 pt-8" style="background-color:aliceblue">
        <div class="w-4/5 mx-auto border-2 bg-blue-200 border-blue-300 m-4 p-2 uppercase text-sm font-semibold rounded-lg shadow-md">{{ user.username }}</div>
        <div class="w-4/5 mx-auto border-2 bg-blue-200 border-blue-300 m-4 p-2 uppercase text-sm font-semibold rounded-lg shadow-md">{{ user.email }}</div>
        <div class="w-4/5 mx-auto border-2 bg-blue-200 border-blue-300 m-4 p-2 uppercase text-sm font-semibold rounded-lg shadow-md">{{ user.address }}</div>
        <div class="w-4/5 mx-auto border-2 bg-blue-200 border-blue-300 m-4 p-2 uppercase text-sm font-semibold rounded-lg shadow-md">{{ user.phone }}</div>
        <div class="w-4/5 mx-auto border-2 bg-blue-200 border-blue-300 m-4 p-2 uppercase text-sm font-semibold rounded-lg shadow-md">{{ user.website }}</div>
        <div class="w-4/5 mx-auto border-2 bg-blue-200 border-blue-300 m-4 p-2 uppercase text-sm font-semibold rounded-lg shadow-md">{{ user.company }}</div>
    </div>    
</template>

<script>
    export default {
        props: ['user']
}
</script>

<style>

</style>