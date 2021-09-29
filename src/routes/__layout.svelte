<script>
  import '../app.css';
</script>

<nav>
  <a href='/'>Home</a>
  <a href='/about'>About</a>
  <a href='/settings'>Settings</a>
</nav>

<main>
  <slot/>
</main>

<style>
  nav {
    position: fixed;
    bottom: 0;
    width: 100%;
    height: 64px;
    background-color: #333;
    display: grid;
    grid-auto-flow: column;
    grid-auto-columns: min-content;
    column-gap: 1rem;
    align-items: center;
    padding: 0 2rem;
    border-top: 1px solid #555;
  }

  a {
    text-decoration: none;
    background-color: #555;
    font-size: 16px;
    padding: 8px 16px;
    border-radius: 3rem;
    color: #eee;
  }

  main {
    padding: 2rem;
  }
</style>