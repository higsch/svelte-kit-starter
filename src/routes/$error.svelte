<script>
  import { dev } from '$app/env';

  export let status;
  export let error;
</script>

<main>
  <h1>{status}</h1>
  <p>Something went wrong!</p>
  {#if (dev)}
    <pre>{error.stack}</pre>
  {/if}
</main>
