<script>
import { onMount } from 'svelte';

export let testRdfdata;
export let testGraph;

testGraph.update(() => ($testRdfdata + ' modified by testV'));

</script>

<div>
<h2>Component testV</h2>
component: {$testGraph}
</div>
