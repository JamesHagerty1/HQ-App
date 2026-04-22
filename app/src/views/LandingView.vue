<script setup lang="ts"></script>

<template>
    <main class="landing">
        <img class="logo" src="/logo.svg" alt="HQ Logo" />
        <p class="tagline">
            A home for your teams and their projects.
        </p>
    </main>
</template>

<style scoped>
    /* Horizontally center logo and tagline, while vertical centering rules are
    placing the bottom of the logo slightly above the center horizontal line
    and placing the top of the paragraph slightly below the center horizontal
    line. */

    .landing {
        position: relative;

        min-height: 100vh;
        width: auto; /* Making default style explicit. */
    }

    .logo {
        position: absolute;
        bottom: calc(50% + 10px);
        left: 50%;
        transform: translateX(-50%);

        width: 200px;
        height: auto;
    }

    .tagline {
        position: absolute;
        top: calc(50% + 10px);
        left: 50%;
        transform: translateX(-50%);

        margin: 0;
        width: 400px;
        height: auto;

        text-align: center;
        line-height: normal;
        letter-spacing: 0.02em;

        font-family: 'Instrument Sans', system-ui, sans-serif;
        font-size: 48px;
    }
</style>
