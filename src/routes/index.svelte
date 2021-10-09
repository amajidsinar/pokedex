<script>
    import {pokemon} from "../stores/pokemart";
    import PokemanCard from "../components/pokemanCard.svelte";

</script>
<svelte:head>
    <title>Svelte Kit Pokedex</title>
</svelte:head>

<h1 class="text-4xl text-center my-8 uppercase">Svelte Kit Pokedex</h1>

<div class="grid gap-4 md:grid-cols-2 grid-cols-1">
    {#each $pokemon as pokeman}
    <PokemanCard pokeman={pokeman}/>
    {/each}
</div>

<style>
    h1{
        color: rgb(187, 149, 149);
    }
</style>
