<script>
  export let operator;
  import PointsCounter from "./PointsCounter.svelte";
</script>

<div class="photo-operator">
  <img src="{operator.profilePicture}" alt="{operator.name}" />
  <h3>{operator.name}</h3>
  <PointsCounter points="{operator.points}" />
</div>