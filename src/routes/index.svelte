<script>
    let routes = [
        {'url': 'contact', 'title': 'Contact'},
    ];
</script>

<main>
    <h1>FOLKE SVERDRUP SAENGER</h1>
    {#each routes as route}
        <a href="/{route.url}">
            {route.title}
        </a>
        <br/>
    {/each}
</main>
