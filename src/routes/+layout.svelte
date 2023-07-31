<!-- Layout.svelte -->

<script>
  export let title;
</script>

<main>
  <nav>
    <ul>
      <li><a href="/Home">Home</a></li>
      <li><a href="/About">About</a></li>
      <li><a href="/Projects">Projects</a></li>
      <li><a href="/Contact">Contact</a></li>
    </ul>
  </nav>
  
  <section class="hero">
    <h1>Gerald L.</h1>
    <p>Tier 1 Incident Response Analyst</p>
  </section>
  
  <section class="content">
    <slot></slot>
  </section>
  
  <footer>
    <p>&copy; 2023 Gerald L. All rights reserved.</p>
  </footer>
</main>

<style>
  main {
    font-family: 'Roboto', sans-serif;
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: auto 1fr auto;
    min-height: 100vh;
    padding: 2rem;
    gap: 2rem;
	}
	body {
  background: linear-gradient(to right, #2a2e35, #12181b);
}

  nav {
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #333;
    padding: 1rem;
    border-radius: 10px;
  }

  ul {
    list-style-type: none;
    display: flex;
    gap: 1rem;
  }

  li {
    font-size: 1.2rem;
  }

  a {
    color: white;
    text-decoration: none;
    padding: 0.5rem 1rem;
    border-radius: 5px;
  }

  .hero {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-color: #1a1a1a;
    color: white;
    text-align: center;
    padding: 4rem 0;
    border-radius: 10px;
  }

  .hero h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
  }

  .hero p {
    font-size: 1.5rem;
    opacity: 0.8;
  }

  .content {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  footer {
    text-align: center;
    padding: 1rem 0;
    background-color: #333;
    color: white;
    border-radius: 10px;
  }
</style>
