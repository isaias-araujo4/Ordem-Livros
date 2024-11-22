<script>
    import ItemAutor from "../../components/autor/itemAutor.svelte";
    import Titulo from "../../components/shared/titulo.svelte";
    import autores from "../../constants/autores";
</script>

<div class="flex flex-col gap-10">
    <Titulo
        principal="Autores"
        secundario="Conheça os autores que escrevem as histórias que voçê ama!"
    />

    <div class="grid grid-cols-2 gap-5">
        {#each autores as autor}
            <ItemAutor {autor} />
        {/each}
    </div>
</div>
