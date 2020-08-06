<script>
  let movie = "Aliens";
  let worstYear = 2020;
</script>

<style>
  section {
    border: 1px solid #ccc;
    padding: 10px 15px;
    margin-bottom: 20px;
  }

  input[type="range"] {
    vertical-align: middle;
    width: 40rem;
  }
</style>

<svelte:head>
  <title>Challenges</title>
</svelte:head>

<h2>Challenges</h2>

<section>
  <h3>
    Item #3: Make a component with an element that changes value with the input
  </h3>
  <label>
    Your favorite movie is:
    <input bind:value={movie} />
  </label>
  <p>Your favorite movie is {movie}</p>
</section>

<section>
  <h3>Item #4: Make a component that changes with range slider input</h3>
  <label>
    Pick the worst year so far:
    <input type="range" bind:value={worstYear} min="1" max="2020" />
  </label>
  <p>The worst year so far is {worstYear}</p>
</section>
