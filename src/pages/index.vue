<script setup lang="ts">
import { ref } from 'vue';

const arr = ref<string[]>([
    "I am an athlete by heart; a disciplined individual who takes any necessary means to produce fast quality results at a higher standard. I've practiced and mastered the skill of adaptability in any situation, which makes my learning curve of learning newer technologies, skill sets, and more come at a faster rate.",
    "My natural ambitions are to solve problems. So far, I have demonstrated histories of working with many businesses to generate more revenue, improve internal business operations, and increase pounds toward athletes' powerlifting total. Currently, I have also possessed a skill that can solve business problems with software solutions. Now, let me solve your problems and help your company grow!",
]);

const video = ref({
    url: '/videos/deadlift.mp4',
    label: "Don't click this!",
    title: 'Sumo deadlift: 655 lbs.',
});
</script>

<template>
    <Card :descriptions="arr" :video="video" />
</template>

<style>
* {
    -ms-overflow-style: none;
    /* Internet Explorer 10+ */
    scrollbar-width: none;
    /* Firefox */
}

*::-webkit-scrollbar {
    display: none;
    /* Safari and Chrome */
}

html {
    overflow: scroll;
    overflow-x: hidden;
}

::-webkit-scrollbar {
    width: 0;
}


body {
    background-color: #0b0a08 !important;
}
</style>
