<script>
  import Logo from './Logo.svelte'
  import Nav from './Nav.svelte'

  export let segment
</script>

<style>
  header {
    display: flex;
    margin: 0 auto;
    padding: 2em;
    width: 100%;
    font-family: 'Titillium Web';
    background-color: #003057;
  }
</style>

<header>
  <Logo />
  <Nav {segment} />
</header>
