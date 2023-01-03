<script setup lang="ts">
import { cards } from '../assets/cards'

</script>

<template>

<div v-for="card in cards" :key="card.name">
    <Card :emoji="card.emoji" :name="card.name" :team="card.team" :powers="card.powers"/>
</div>

</template>

<route lang="yaml">
    name: all-cards
    </route>
    