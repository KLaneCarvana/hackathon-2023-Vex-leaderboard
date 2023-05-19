<script>
  import PhotoOperator from "./PhotoOperator.svelte";
  let operators = []; // Fetch the data here, e.g., from an API

  operators.sort((a, b) => b.points - a.points);
</script>

<div class="leaderboard">
  {#each operators as operator (operator.id)}
    <PhotoOperator {operator} />
  {/each}
</div>