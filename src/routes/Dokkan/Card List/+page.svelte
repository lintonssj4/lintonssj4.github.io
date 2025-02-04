<script>
    import CardsDokkan from '$lib/components/CardsDokkan.svelte';
    import {dokkancards} from '$lib/data.js';
</script>

<div class="row g-4">
    {#each dokkancards as card}
      <div class="col">
        <CardsDokkan {...card} />
      </div>
    {/each}
  </div>