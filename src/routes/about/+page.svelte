<svelte:head>
  <title>CleeSim — About</title>
  <meta name="title" content="CleeSim — About" />
  <link
    href="https://fonts.googleapis.com/css2?family=Kanit&display=swap"
    rel="stylesheet"
  />
</svelte:head>

<div class="container">
  <main class="center">
    <h1>About</h1>
    <pre>We're an independent Roblox game development team. With over 4 years of experience behind our backs, we're aiming to create the best games on Roblox, where players have a fulfilling and fun experience. This is where games are made with passion and love.</pre>

    <div class="team">
      <a href="https://www.roblox.com/users/142642210/profile" class="tooltip">
        <img src="/team/gergo135.png" alt="gergo135" class="rounded-image" />
        <span class="tooltip-text">gergo135</span>
      </a>
      <a href="https://iku.pet/" class="tooltip">
        <img src="/team/iku.pet.png" alt="iku.pet" class="rounded-image" />
        <span class="tooltip-text">iku.pet</span>
      </a>
      <a href="https://www.roblox.com/users/1658640475/profile" class="tooltip">
        <img
          src="/team/devsmartie.png"
          alt="devsmartie"
          class="rounded-image"
        />
        <span class="tooltip-text">devsmartie</span>
      </a>
      <!-- <a href="https://www.roblox.com/users/606074553/profile" class="tooltip">
                <img src="/team/trudaw.png" alt="trudaw" class="rounded-image">
                <span class="tooltip-text">trudaw</span>
            </a> -->
      <a href="https://www.roblox.com/users/4235996651/profile" class="tooltip">
        <img
          src="/team/that.one.beni.png"
          alt="that.one.beni"
          class="rounded-image"
        />
        <span class="tooltip-text">🕊️ 02/14/2024 Long Live Beni</span>
      </a>
      <a href="https://www.roblox.com/users/1083454399/profile" class="tooltip">
        <img
          src="/team/shadow1409.png"
          alt="shadow1409"
          class="rounded-image"
        />
        <span class="tooltip-text">shadow1409</span>
      </a>
      <a href="https://www.roblox.com/users/1154481085/profile" class="tooltip">
        <img
          src="/team/masterkyllian8.png"
          alt="masterkyllian8"
          class="rounded-image"
        />
        <span class="tooltip-text">masterkyllian8</span>
      </a>
    </div>
  </main>
</div>

<style>
  .container {
    max-width: 900px;
    padding: 0;
    display: flex;
    justify-content: center;
    font-family: "Kanit", sans-serif;
    font-weight: bold;
  }

  main {
    max-width: 100%;
    min-height: 500px;
    text-align: left;
    margin: 0 auto;
    box-sizing: border-box;
    font-family: "Kanit", sans-serif;
    font-weight: bold;
  }

  h1 {
    font-weight: 700;
    margin: 0 0 50px 0;
    font-size: 36px;
    text-align: center;
    font-family: "Kanit", sans-serif;
    font-weight: bold;
  }

  pre {
    white-space: pre-wrap;
    white-space: -moz-pre-wrap;
    white-space: -pre-wrap;
    white-space: -o-pre-wrap;
    word-wrap: break-word;
    font-family: "Kanit", sans-serif;
    font-weight: bold;
  }

  .team {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
  }

  .rounded-image {
    border-radius: 50%;
    cursor: pointer;
    width: 128px;
    height: 128px;
  }

  @media (max-width: 600px) {
    .rounded-image {
      width: 64px;
      height: 64px;
    }
  }

  .tooltip {
    position: relative;
  }

  .tooltip-text {
    visibility: hidden;
    width: 120px;
    background-color: #000;
    color: #fff;
    text-align: center;
    border-radius: 6px;
    padding: 5px;
    position: absolute;
    z-index: 1;
    bottom: 125%;
    left: 50%;
    transform: translateX(-50%);
    opacity: 0;
    transition: opacity 0.3s;
  }

  .tooltip:hover .tooltip-text {
    visibility: visible;
    opacity: 1;
  }
</style>
