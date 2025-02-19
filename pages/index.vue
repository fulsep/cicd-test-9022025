<script setup lang="ts">
let {data: users}: any = await useFetch("http://146.190.108.44:8888/users")
</script>

<template>
    <h1>List users</h1>
    <ul>
            <li v-for="user in users">
            {{ user.name }}
            {{ user.email }}
            </li>
    </ul>
</template>