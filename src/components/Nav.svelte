<script>
  export let segment;
</script>

<style>
  nav {
    align-items: flex-end;
    display: flex;
    flex: 1;
    font-family: 'Titillium Web';
    font-weight: 700;
    justify-content: flex-end;
    text-transform: uppercase;
  }

  a {
    color: white;
    text-decoration: none;
    padding: 10px 5px;
    display: block;
    position: relative;
    margin-left: 20px;
  }

  a:not(.selected) {
    opacity: 0.7;
  }

  a::before {
    content: '';
    position: absolute;
    transition: transform .3s ease;
    left: 0;
    bottom: 0;
    width: 100%;
    height: 2px;
    background: #AAA;
    transform: scaleX(0);
  }

  a:hover::before,
  .selected::before {
    transform: scaleX(1);
  }

  .selected::before {
    background: #F38F1D;
  }
</style>

<nav>
  <a class='{segment === undefined ? "selected" : ""}' href='.'>home</a>
  <a class='{segment === "about" ? "selected" : ""}' href='about'>about us</a>
  <a rel=prefetch class='{segment === "blog" ? "selected" : ""}' href='blog'>blog</a>
</nav>
