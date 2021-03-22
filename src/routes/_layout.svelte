<script>
  import * as Sapper from "@sapper/app";

  const { preloading } = Sapper.stores();
</script>

<main>
  <slot />
  {#if $preloading}
    <p>Currenting Preloading...</p>
  {/if}
</main>
