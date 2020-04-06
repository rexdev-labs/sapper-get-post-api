<script>
    function getSomething(){
        fetch('getapi')
    }
</script>


<svelte:head>
    <title>Get Page</title>
</svelte:head>

<h1>
    This Is Get Page
</h1>

<button on:click={getSomething}>Get Data</button>