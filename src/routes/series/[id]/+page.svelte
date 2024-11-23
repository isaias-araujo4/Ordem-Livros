<script>
    import {page} from "$app/stores"
    import ConteudoSerie from "../../../components/serie/conteudoSerie.svelte";
    
</script>

<ConteudoSerie serie={$page.data.serie}/>