<script lang="ts">
    export let serie: any = null;
</script>

{#if serie}
    <a href="/series/{serie.id}" class="flex flex-col rounded-md overflow-hidden">
        <img src={serie.imagem} alt="imagem da serie" class="h-96 object-cover">
        <div class="flex flex-col gap-2 p-5">
            <span class="text-2xl font-black">{serie.titulo}</span>
            <span class="text-sm text-zinc-400 text-justify">{serie.descricao}</span>
            <button class="flex justify-center items-center gap-2 py-1 px-8 rounded-md bg-blue-500 text-white hover:bg-blue-600 ">Leia mais</button>
        </div>
    </a>
{/if}


