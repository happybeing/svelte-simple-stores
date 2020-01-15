<script>
  import TestR from "./TestR.svelte";
  import TestV from "./TestV.svelte";
  import TestG from "./TestG.svelte";

  import { writable } from "svelte/store";

  export const testRdfdata = writable(0);
  export let testGraph = writable(0);

</script>

<style>
	h1 {
		color: purple;
	}
</style>

<h1>Svelte Simple Stores Example</h1>
<p><TestR {testRdfdata}/>App TestR: {$testRdfdata}</p>
<p><TestV {testRdfdata} {testGraph}/>App TestV: testRdfdata: {$testRdfdata}<br/>App TestV: testGraph: {$testGraph}</p>
<p><TestG {testGraph}/>App TestG: testGraph: {$testGraph}</p>
