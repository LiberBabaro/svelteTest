<script>
	import SomeBlocks from './SomeBlocks.svelte';
	import Block from "./Block.svelte";

	const blockSettings = {
	    color: 'black',
        opacity: '0.7'
    };
</script>
<Block {...blockSettings}/>
<SomeBlocks/>