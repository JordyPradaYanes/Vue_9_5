<script setup>

import { ref } from "vue";
const val = ref(false);

const items = ["Opcion 1","Opcion 2","Opcion 3","Opcion 4"];

</script>

<template>

    <ul v-show="val">
        <li v-for="(items,index) in items">
            {{ items }}
        </li>
    </ul>
    <button class=" m-20 absolute right-0 bottom-0 flex justify-center items-center size-10 rounded-full bg-red-500 text-white" @click="val = !val">
    </button>
    
</template>
