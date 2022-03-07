<script setup>
import useAuth from "../composables/useAuth";
const { isAuthenticated, user } = useAuth();
</script>

<template>
<div class ="flex flex-col space-y-12 items-center justify-center min-h-screen-nonav">
    <h2 v-if="!isAuthenticated" class="text-6xl tracking-tighter font-extralight">Welcome<span ></span></h2>
    <h2 v-else class="text-6xl tracking-tighter font-extralight">Welcome {{ user }}<span ></span></h2> 
<img src="../assets/bgindex.png" alt="Hello BG" >  
</div>

</template>
