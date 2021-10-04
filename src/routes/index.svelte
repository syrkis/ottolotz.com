<script>
    let routes = [
        {'url': 'seven', 'title': 'Seven sages laid its foundations'},
        {'url': 'sun', 'title': 'The sun hitches up her skirt for Utnapishtim'},
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
