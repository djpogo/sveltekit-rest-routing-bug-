<script context="module">
  export async function load({page}) {
    return {
        props: {
            pagePath: page.path,
        }
    };
  }
</script>

<script>
    export let pagePath;
</script>

<pre>page path is {pagePath}</pre>