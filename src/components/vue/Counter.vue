<script setup>
import { ref } from 'vue'
    let count = ref(0);

    function addValue(){
        count.value ++;
        console.log(count)
    }
</script>

<template>
    <div @click="addValue"  class="bg-blue-500 text-white py-2 px-4 rounded inline-block hover:cursor-pointer hover:bg-blue-600 transition-colors">
        ¡Presioname! {{ count }}
    </div>

</template>