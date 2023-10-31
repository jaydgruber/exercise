<!--
  https://shoelace.style/components/details#grouping-details
  intend to make a component that groups several exercises, which are `sl-details`
  but only one of them can be expanded at a time
-->
<script>
  import { onMount } from "svelte";

  let card;
  onMount(() => {
    card.addEventListener('sl-show', event => {
      if (event.target.localName === 'sl-details') {
        [...card.querySelectorAll('sl-details')].map(details => (details.open = event.target === details));
      }
    });
  });
</script>

<sl-card bind:this={card}>
  <slot></slot>
</sl-card>