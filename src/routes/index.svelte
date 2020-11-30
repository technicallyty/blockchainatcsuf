<script>

import About from "./about.svelte";

</script>
<style>
  .home-container {
    align-items: center;
    display: flex;
    flex: 1;
    justify-content: center;
    margin: 10em 0;
    min-height: 400px;
    padding-bottom: 150px;
    font-family: 'Titillium Web';
  }

  wrap {
    display: block;
  }


  .home-copy {
    flex: 1;
  }

  h1 {
    font-family: 'Titillium Web';
    font-weight: 700;
    margin-bottom: 0.5em;
    color: #F38F1D;
  }

  p {
    font-size: 1.4em;
    line-height: 1.5;
    font-weight: bolder;
  }

  figure {
    margin: 0 1em;
    text-align: center;
  }

  figcaption {
    font-size: .8em;
    font-style: italic;
  }

  img {
    width: 100%;
    max-width: 400px;
  }

  .container {
    display: flex;
    align-items: center;
    flex-direction: row;
    justify-content: center;
    min-width: 100%;
  }
  
  .spacer {
    margin: 0px 0;
  }

  .csuf-college-blue {
    color: #003057;
  }
  
  .center-heading {
    text-align: center;
  }

  .join {
    padding: .3em 1em;
    border: 2px solid;
    border-radius: 3px;
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    font-size: 20px;
    font-weight: 500;
    line-height: 1.7em;
    cursor: pointer;
    text-decoration: none;
  }

  @media (max-width: 1020px) {
    p {
      font-size: 1.2em;
    }

    img {
      max-width: 300px;
    }
  }

  @media (max-width: 800px) {
    .home-container {
      flex-direction: column;
    }

    .home-copy {
      flex: 0;
      padding-bottom: 2em;
      text-align: center;
    }
  }

  .banner {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .banner-img {
    border-radius: 30px;
    max-height: 200px;
  }
  .event-description > h2 {
    font-family: 'Merriweather';
  }
  .event-container {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    min-width: 1400px;
    margin: 5em 5em;
    text-align: start;
    align-items: center;
  }
  .event-description {
    max-width: 600px;
  }
  hr.solid {
  border-top: 3px solid #bbb;
  width: 100%;
}
</style>

<svelte:head>
  <title>Blockchain at CSUF</title>
</svelte:head>

<div class="home-container">
  <div class="home-copy">
    <h1>Blockchain at <span class="csuf-college-blue">CSUF</span>.</h1>
    <wrap>
      <p>CSUF's hub for all things blockchain.</p>
      <a class="join" href="https://fullerton.campuslabs.com/engage/" target="_blank">Join Us</a>
    </wrap>
  </div>

  <figure>
    <img alt='Person typing on laptop' src='undraw-illustration.svg'>
    <figcaption>Illustration thanks to <a href="https://undraw.co" target="_blank">Undraw</a></figcaption>
  </figure>
</div>


<div class="spacer" />
<h1 class="center-heading">Past Events</h1>
<div class="banner">
  <div class="event-container">
    <div class="event-description">
      <h2>HackFS</h2>
      <p>Students at HackFS built a new decentralized finance protocol that enabled liquidity pools to borrow and lend.</p>
    </div>
    <img class="banner-img" src="hackfs.png" alt="Hack FS">
  </div>
  <hr class="solid">
  <div class="event-container">
    <img src="ETHOnline.png" alt="EthOnline Banner" class="banner-img">
    <div class="event-description">
      <h2>ETHOnline Hackathon</h2>
      <p>Students built a new protocol that enabled DeFi users to stake coins in an offchain protocol.</p>
    </div>
  </div>
  <hr class="solid">
  <div class="event-container">
    <div class="event-description">
      <h2>CSUF Annual Gitcoin Bounty</h2>
      <p>Students claimed and completed bounties at our annual gitcoin hackathon - a CSUF exclusive event.</p>
    </div>
    <img src="gitcoin.jpg" alt="gitcoin" class="banner-img">
  </div>
</div>