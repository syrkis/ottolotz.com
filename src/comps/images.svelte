<script>
    
    import Image from './image.svelte'; 

    import axios from 'axios';
    import { onMount } from 'svelte';

    export let project;
    let works = [];

    async function getWork() {
        const res = await axios.get(`https://files.thortaohansen.com/${project}/index.json`);
        return res.data
    }

    onMount(async () => {
        const res = await getWork();
        works = await res.works;
    });

</script>

<div>

    {#each works as work, i}
        <Image url='https://files.thortaohansen.com/{project}/{i}.jpg' />
        {work.title}<br/>
        {work.year}<br/>
        {work.dimensions}<br/>
        {work.materials}
    {:else}
        ...loading
    {/each}

</div>
