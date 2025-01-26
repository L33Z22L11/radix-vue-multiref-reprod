<script setup lang="ts">
import { TooltipProvider, TooltipRoot, TooltipTrigger } from 'radix-vue'
</script>

<template>
    <TooltipProvider>
        <TooltipRoot>
            <TooltipTrigger as-child>
                <slot />
            </TooltipTrigger>
        </TooltipRoot>
    </TooltipProvider>
</template>