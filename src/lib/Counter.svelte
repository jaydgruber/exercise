<script>
  let count = 0
  const increment = () => {
    count += 1
  }
  const handleKeyDown = (event) => {
    if (["Enter", "Space"].includes(event?.code)) return increment();
  }
</script>

<sl-button variant="primary" pill="pill" size="medium" role="button" tabindex="0" on:click={increment} on:keydown={handleKeyDown}>
  <sl-icon slot="prefix" name="plus-circle"></sl-icon>
  {count}
</sl-button>
