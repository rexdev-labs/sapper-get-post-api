<script>
    let data = 'yumy';
    function postSomething(){
        fetch('postapi',{
            method: 'POST',
            headers:{
                'Content-Type': 'application/json'
            },
            body: JSON.stringify({
                data
            })
        })
    }

</script>

<svelte:head>
    <title>Post Page</title>
</svelte:head>

<h1>
    This Is Post Page
</h1>



<input bind:value="{data}">

<button on:click={postSomething}>Post Data</button>