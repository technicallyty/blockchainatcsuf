<script>

import { fix_and_outro_and_destroy_block } from "svelte/internal";

</script>
<style>
  .container {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  h1 {
    text-align: center;
    margin: 0;
  }
  h1 > span {
    color: #F38F1D;
  }

  .team-container {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    width: 1200px;
    align-content: center;
    justify-content: space-between;
  }
  
  .team-card {
    display: flex;
    flex-direction: column;
    min-height: 500px;
    width: 500px;
    margin: 25px;
  }

  .team-header { 
    display: flex;
    flex-direction: row;
  }


  .team-header > img {
    border-radius: 30px;
    height: 200px;
    width: 200px; 
    object-fit: contain;
  }
  .team-info{
    display: flex;
    flex-direction: column;
  }

  .name {
    color: black;
  }

  .team-info > ul {
    list-style: none;
    display: flex;
    flex-direction: row;
  }
  .team-info > ul li {
    margin: 0 15px;
  }

  p {
    color: black;
  }

  .about-text {
    margin-bottom: 100px;
  }
</style>

<svelte:head>
  <title>About</title>
</svelte:head>

<div class="container">
  <h1>Who <span>We</span> Are</h1>
  <p class="about-text">
    We are a group of students with backgrounds in finance, blockchain, security,
    and P2P networks. We all share a passion for the decentralized web and financial liberation through cryptocurrencies. 
  </p>
  <h1>Our Team</h1>
  <div class="team-container">
  <div class="team">
    <div class="team-card">
      <div class="team-header">
        <img src="myself.png" alt="Tyler Goodman" >
        <div class="team-info">
          <h2 class="name">Tyler Goodman</h2>
          <ul>
            <li><img src="github.png" alt="github"></li>
            <li><img src="twitter.png" alt="twitter"></li>
          </ul>
        </div>
      </div>
      <p>President/Founder of Blockchain at CSUF. Software Engineer in the IT/AppDev department at CSUF. Ethereum Core contributor. DeFi enthusiast. I enjoy working with Golang, Solidity, and React with Web3.</p>
    </div>
  </div>
  <div class="team">
    <div class="team-card">
      <div class="team-header">
        <img src="myself.png" alt="Tyler Goodman" >
        <div class="team-info">
          <h2 class="name">Tyler Goodman</h2>
          <ul>
            <li><img src="github.png" alt="github"></li>
            <li><img src="twitter.png" alt="twitter"></li>
          </ul>
        </div>
      </div>
      <p>President/Founder of Blockchain at CSUF. Software Engineer in the IT/AppDev department at CSUF. Ethereum Core contributor. DeFi enthusiast. I enjoy working with Golang, Solidity, and React with Web3.</p>
    </div>
  </div>
  <div class="team">
    <div class="team-card">
      <div class="team-header">
        <img src="myself.png" alt="Tyler Goodman" >
        <div class="team-info">
          <h2 class="name">Tyler Goodman</h2>
          <ul>
            <li><img src="github.png" alt="github"></li>
            <li><img src="twitter.png" alt="twitter"></li>
          </ul>
        </div>
      </div>
      <p>President/Founder of Blockchain at CSUF. Software Engineer in the IT/AppDev department at CSUF. Ethereum Core contributor. DeFi enthusiast. I enjoy working with Golang, Solidity, and React with Web3.</p>
    </div>
  </div>
  <div class="team">
    <div class="team-card">
      <div class="team-header">
        <img src="myself.png" alt="Tyler Goodman" >
        <div class="team-info">
          <h2 class="name">Tyler Goodman</h2>
          <ul>
            <li><img src="github.png" alt="github"></li>
            <li><img src="twitter.png" alt="twitter"></li>
          </ul>
        </div>
      </div>
      <p>President/Founder of Blockchain at CSUF. Software Engineer in the IT/AppDev department at CSUF. Ethereum Core contributor. DeFi enthusiast. I enjoy working with Golang, Solidity, and React with Web3.</p>
    </div>
  </div>
</div>
</div>
