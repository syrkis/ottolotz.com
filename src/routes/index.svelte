<script>
    let routes = [
        {'url': 'articles', 'title': 'Written works'},
        {'url': 'contact', 'title': 'Contact'},
    ];
</script>

<main>
    <h1>FOLKE SVERDRUP SAENGER</h1>
    <p>folke@sverdrupsaenger.com, 0045 50318037.</p>
    <br/> 
    <p>twitter/sverdrupsaenger, twitch.tv/erauqs, IG: folkesverdrup and contentbasedlifestyles.</p>
    <br/>
    <p>Sign up for the erauqs newsletter at newsletter@erauqs.com when it launches (near future).</p>
    {#each routes as route}
        <a href="/{route.url}">
            {route.title}
        </a>
        <br/>
    {/each}
</main>
