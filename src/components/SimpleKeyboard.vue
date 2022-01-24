<template>
    <div class="simple-keyboard"> </div>
</template>

<script setup>
import Keyboard from "simple-keyboard";
import "simple-keyboard/build/css/index.css";

import { ref, onMounted, watch } from "vue";

const keyboard = ref(null);

onMounted(() => {
  keyboard.value = new Keyboard();
});

</script>