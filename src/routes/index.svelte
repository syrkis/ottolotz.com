<script>
    let routes = [
        {'url': 'articles', 'title': 'Written works'},
        {'url': 'contact', 'title': 'Contact'},
    ];
</script>

<main>
    <h1>FOLKE SVERDRUP SAENGER</h1>
    <p>folke@sverdrupsaenger.com, architect and editor at large</p>
    
    <br/> 
    {#each routes as route}
        <a href="/{route.url}">
            {route.title}
        </a>
        <br/>
    {/each}
</main>
