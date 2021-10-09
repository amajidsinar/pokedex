<script>
    import {pokemon} from "../stores/pokemart"
</script>
<svelte:head>
    <title>Svelte Kit Pokedex</title>
</svelte:head>

<h1 class="text-center">Svelte Kit Pokedex</h1>

{#each $pokemon as pokeman}
<p>{pokeman.name}</p>
{/each}

<style>
    h1{
        color: rgb(187, 149, 149);
    }
</style>
