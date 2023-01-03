<script setup lang="ts">
// const props = defineProps<{
//     name: string;
//     emoji: string;
//     powers?: string[];
//     team: string;
//   }>()
const props = defineProps({
    name: String,
    emoji: String,
    powers: Array,
    team: String 
})

</script>

<template>
      <div class="bg-violet-300 border-4 m-4  border-gray-800 h-96 max-w-sm flex flex-col items-center justify-around">
      <h1 class="text-4xl py-3 font-bold">{{props.name}}</h1>
      <h1 class="text-8xl py-3 align-middle">{{props.emoji}}</h1>
      
      <p v-if="props.powers" class="p-2">Powers: {{props.powers.join(", ")}}</p> 
    
    </div>
</template>