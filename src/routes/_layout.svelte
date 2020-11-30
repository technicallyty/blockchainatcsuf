<script>
  import Header from '../components/Header.svelte';

  export let segment;
</script>

<style>
  .layout {
    display: flex;
    flex-direction: column;
    min-height: 100%;
    min-height: 100vh;
    background-color: white;
  }

  main {
    flex: 1;
    position: relative;
    margin: 0 auto;
    max-width: 1400px;
    background-color: white;
    padding: 1em 2em;
    box-sizing: border-box;
    width: 100%;
    display: flex;
    flex-direction: column;
    font-family: 'Titillium Web';
  }

  footer {
    display: flex;
    justify-content: space-around;
    align-items: center;
    color: #AAA;
    font-size: 1em;
    font-family: Rubik, sans-serif;
    margin: 5em auto 0 auto;
    text-align: center;
    width: 100%;
    background-color:#F38F1D;
  }
  h2 {
    font-family: 'Titillium Web';
    text-align: center;
    margin: auto 0;
    color: white;
  }
  ul{
    display: flex;
    flex-direction: row;
    list-style: none;
  } 

  li {
    margin: 0 30px;
    cursor: pointer;
  }
</style>

<div class="layout">
  <Header {segment}/>

  <main>
    <slot></slot>
  </main>

  <footer>
    <div>
      <h2>Blockchain at CSUF</h2>
    </div>
    <div>
      <ul>
        <li><img src="discord.png" alt="discord"/></li>
        <li><img src="instagram.png" alt="instagram"/></li>     
        <li><img src="twitter.png" alt="twitter"/></li>   
        <li><img src="github.png" alt="github"/></li>  
      </ul>
    </div>
  </footer>
</div>
