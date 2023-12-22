<script lang="ts">
    import type { PageData } from './$types';
	import DataTable from "./data-table.svelte";    
    export let data: PageData;
	$: tracks_entries = data.tracks_entries;

</script>

<div class="container mx-auto w-1/2 py-10">
	<DataTable tracks={tracks_entries}
	/>
</div>