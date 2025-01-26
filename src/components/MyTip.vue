<script setup lang="ts">
import { TooltipProvider, TooltipRoot, TooltipTrigger } from 'radix-vue'
import { useTemplateRef, watchEffect } from 'vue'

const btn = useTemplateRef('btn')

watchEffect(() => {
    console.log(btn.value)
})
</script>

<template>
    <TooltipProvider>
        <TooltipRoot>
            <TooltipTrigger asChild>
                <button ref="btn">Hover me</button>
            </TooltipTrigger>
        </TooltipRoot>
    </TooltipProvider>
</template>