<script>
    import {page} from '$app/stores';

    const slug = $page.params.slug;
    const slugArr = $page.params.slug.split('/');
    console.log(slugArr);
</script>

<h1>Docs Home Page</h1>
<p>Slug: {slug}</p>

{#if slugArr.length === 1}
    <p>Viewing docs for feature: {slugArr[0]}</p>
{:else if slugArr.length === 2}
    <p>Viewing docs for feature {slugArr[0] } and concept {slugArr[1]}</p>
{/if}