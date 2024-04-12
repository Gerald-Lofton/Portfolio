<script>
  function goto(path) {
    console.log(`Navigating to ${path}`);
  }
</script>

<div class="layout">
  <header>
    <nav>
      <ul>
        <li><a href="/Home" on:click={() => goto('/Home')}>Home</a></li>
        <li><a href="/About" on:click={() => goto('/About')}>About</a></li>
        <li><a href="/Projects" on:click={() => goto('/Projects')}>Projects</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <slot></slot>
  </main>

  <footer>
    <p>&copy; 2023 Gerald L. All rights reserved.</p>
  </footer>
</div>

<style>
  .layout {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
  }

  header {
    background-color: #333;
    padding: 1rem;
    position: sticky;
    top: 0;
    z-index: 1;
  }

  nav {
    display: flex;
    justify-content: center;
  }

  ul {
    list-style-type: none;
    display: flex;
    gap: 1rem;
  }

  a {
    color: white;
    text-decoration: none;
    padding: 0.5rem 1rem;
    border-radius: 5px;
  }

  a:hover {
    background-color: #555;
  }

  main {
    flex-grow: 1;
    padding: 2rem;
  }

  footer {
    text-align: center;
    padding: 1rem 0;
    background-color: #333;
    color: white;
  }
</style>