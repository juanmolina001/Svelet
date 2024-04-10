<script>
  import Paises from "./lib/paises.svelte";
  const lista=["colombia","venezuela","ecuador","peru","brasil","argentina", "chile", "uruguay", "bolivia", ""]
</script>
<div class="main">
  {#each lista as pais}
    <div>
      <Paises {pais}/>
    </div>
  {:else}
    No existen elementos
  {/each}
</div>
<svelte:head>
  <litle>Paises de suramerica</litle>
</svelte:head>
<style>
  .main {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-gap: 1opx;
    grid-auto-rows: minmax(100px, auto);
  }
</style>