<script>
  import { onMount } from 'svelte';

  onMount(async () => {
    await import('./example.js');
  });

  let count = 0
  const increment = () => {
    count += 1
  }
</script>

<button on:click={increment}>
  count is {count}
</button>

<style>
  button {
    color: red;
  }
</style>
