<script setup lang="ts">
import { useTemplateRef, watchEffect } from "vue";

import MyTip from "./MyTip.vue";
const btn = useTemplateRef('btn')

watchEffect(() => {
    console.log(btn.value)
})
</script>

<template>
    <MyTip>
        <button ref="btn">Hover me</button>
    </MyTip>

</template>