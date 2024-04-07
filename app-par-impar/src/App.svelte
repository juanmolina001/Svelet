<script>
  import Parlmpar from "./lib/ParImpar.svelte";
  let valor=0;
  const listenImput = (event) => valor = event.target.value
</script>
<main>
  <Parlmpar numero={valor}/>
  <input value={valor} on:input={listenImput}>
</main>