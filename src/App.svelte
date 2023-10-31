<script>
  import Counter from './lib/Counter.svelte'
  import Exercise from './lib/Exercise.svelte';
  import Weight from './lib/Weight.svelte'
</script>

<h1>Vite + Svelte</h1>

<sl-card>
  <Counter />
  <Weight />
  <Exercise type="Squats" />
</sl-card>
