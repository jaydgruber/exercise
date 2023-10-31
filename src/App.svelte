<script>
  import Counter from './lib/Counter.svelte'
  import Exercise from './lib/Exercise.svelte';
  import ExerciseGroup from './lib/ExerciseGroup.svelte';
  import Weight from './lib/Weight.svelte'
</script>

<h1>Vite + Svelte</h1>

<sl-card>
  <Counter />
  <Weight />
  <ExerciseGroup>
    <Exercise type="Squats" />
    <Exercise type="Bench press" />
  </ExerciseGroup>
</sl-card>
