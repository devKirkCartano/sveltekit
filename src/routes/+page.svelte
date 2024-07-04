<script>
    import {goto, beforeNavigate, afterNavigate} from '$app/navigation';

    const handleClick = () => {
        console.log('Placing your order')
        goto('/product');
    }
    beforeNavigate((navigation) => {
        console.log({before: navigation})
    })
    afterNavigate((navigation) => {
        console.log({after: navigation})
    })
</script>


<h1>Welcome Home</h1>
<a href="/blog">Blog</a>
<a href="/docs">Docs</a>
<a href="/product">Product</a>
<a href="/marketing">Marketing</a>
<button on:click={handleClick}>Place order</button>