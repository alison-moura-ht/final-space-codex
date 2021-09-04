<template>
    <div class="bg-white p-7 rounded-md m-5">
        <img
            :src="character.img_url"
            alt="Character's image"
            class="border-gray-500 border-solid border-2 w-20 h-20 rounded-full"
        />
        <p class="text-md text-gray-400 mt-2">#{{ character.id }}</p>
        <p class="bold text-lg">{{ character.name }}</p>
        <p
            :class="[
                { 'bg-green-500': character.status.includes('Alive') },
                { 'bg-red-500': character.status.includes('Deceased') },
                { 'bg-gray-800': character.status.includes('Destroyed') },
                { 'bg-yellow-500': character.status.includes('Imprisoned') },
                { 'bg-blue-500': character.status.includes('Operational') },
                'bg-gray-300 text-sm inline-block rounded-full px-3 py-1 text-white'
            ]"
        >{{ character.status }}</p>
        <p class="text-gray-700 text-sm mt-2">{{ character.species }}</p>
    </div>
</template>

<script setup>
import { defineProps } from "vue"

defineProps(["character"])
</script>