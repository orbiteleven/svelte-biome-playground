# Svelte x Biome.js Problems

This is a small repo to show problems encountered when trying to use [Biome.js](https://biomejs.dev) on [Svelte](https://svelte.dev). The simple problem is that when using a component or enum as a type in the `<script>` block, Biome will complain that it should be imported with `type` because it's not seeing that the values are used in the Svelte block. See [src/lib/app.svelte](src/lib/app.svelte)
