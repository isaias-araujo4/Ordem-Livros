<script lang="ts">
    export let livro: any = null;
    import {IconBrandAmazon} from "@tabler/icons-svelte"
</script>

{#if livro}
    <a href={livro.link} target="_blank" class="flex flex-col rounded-md overflow-hidden bg-zinc-800">
        <img src={livro.imagem} alt="imagem do livro" class="h-96">
        <div class="flex-1 flex flex-col p-5 gap-2">
            <span class="flex-1 font-bold text-center">{livro.titulo}</span>
            <button class="flex justify-center items-center gap-2 py-1 px-8 rounded-md bg-blue-500 text-white hover:bg-blue-600 ">
                <IconBrandAmazon size={25}/>
                <span>Link do livro</span>
            </button>
        </div>
    </a>
{/if}
