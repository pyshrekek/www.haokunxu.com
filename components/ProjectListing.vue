<template>
    <NuxtLink :to="project.link" class="card text-center proj-card">
        <img :src="project.image" alt="alt text stub" class="portfolio-img">
        <div class="flex flex-col place-content-center">
            <div class="card-position">
                <p>{{ project.time }}</p>
            </div>
            <h3 class="card-title">{{ project.title }}</h3>
            <p class="card-details">{{ project.desc }}</p>
        </div>
    </NuxtLink>
</template>

<script setup>
    const { project } = defineProps(['project'])
</script>

<style scoped>
</style>