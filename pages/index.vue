<script setup lang="ts">
let {data: users}: any = await useFetch("https://jsonplaceholder.typicode.com/users")
</script>

<template>
    <ul>
            <li v-for="user in users">
            {{ user.name }}
            {{ user.email }}
            </li>
    </ul>
</template>