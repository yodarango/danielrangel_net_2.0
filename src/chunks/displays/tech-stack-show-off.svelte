<script>
  export let techStack = [];
  export let git = "";
  export let url = "";
</script>

<div>
  <h3>Tech Stack</h3>
  <div class="icon-wrapper">
    {#each techStack as item}
      <img src={item} alt="programing language icon" class="icon" />
    {/each}
  </div>
  <div class="links-wrapper">
    <a href={git} target="_blank" rel="noopener noreferrer">Go Git It</a>
    <a href={url} target="_blank" rel="noopener noreferrer">See It Live</a>
  </div>
</div>

<style>
  .icon-wrapper {
    width: 100%;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: space-around;
    flex-wrap: wrap;
  }

  h3 {
    font-size: 3rem;
    width: 100%;
    text-align: center;
    margin: 2rem auto;
  }

  .icon {
    width: 5rem;
    height: 5rem;
    object-fit: cover;
    object-position: center;
    margin: 1rem 0.5rem;
  }

  .links-wrapper {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    transform: translateY(2rem);
  }

  .links-wrapper a {
    display: block;
    margin: 0 2rem;
    font-weight: 900;
    text-decoration: underline;
  }

  @media (max-width: 370px) {
    .icon {
      margin: 0 1rem;
    }
  }

  @media (max-height: 700px) {
    .icon {
      width: 3rem;
      height: 3rem;
    }

    .links-wrapper {
      transform: translateY(0);
      margin: 0.5rem 0.5rem;
    }
  }
  @media (max-width: 500px) {
    .icon {
      width: 3rem;
      height: 3rem;
    }

    .links-wrapper {
      transform: translateY(0);
      margin: 0.5rem 0.5rem;
    }
  }
</style>
