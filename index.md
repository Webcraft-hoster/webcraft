---
layout: default
title: Webcraft Launcher
---

<link href="https://fonts.cdnfonts.com/css/minecraftia" rel="stylesheet">

<style>
  body {
    margin: 0;
    padding: 0;
    background: url('https://feedback.minecraft.net/hc/article_attachments/35363543357965') no-repeat center center fixed;
    background-size: cover;
    font-family: 'Minecraftia', monospace;
    color: #ffffff;
  }

  .overlay {
    background-color: rgba(0, 0, 0, 0.75);
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
  }

  .title {
    font-size: 3em;
    color: #00c853;
    margin-top: 40px;
    text-shadow: 2px 2px #000;
  }

  .content-box {
    background-color: #2d2d2d;
    border-radius: 10px;
    padding: 30px;
    max-width: 600px;
    width: 90%;
    text-align: center;
    box-shadow: 0 0 25px rgba(0, 0, 0, 0.8);
  }

  .play-bar {
    background-color: #1e1e1e;
    width: 100%;
    max-width: 600px;
    padding: 10px 20px;
    border-radius: 0 0 10px 10px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    position: relative;
  }

  .version-selector {
    position: relative;
  }

  .version-selector select {
    background-color: #3a3a3a;
    color: #ffffff;
    border: 2px solid #555;
    font-family: 'Minecraftia', monospace;
    padding: 6px 12px;
    border-radius: 5px;
    appearance: none;
  }

  .play-button {
    background-color: #00c853;
    color: #fff;
    border: none;
    font-family: 'Minecraftia', monospace;
    font-size: 1.2em;
    padding: 10px 40px;
    border-radius: 5px;
    cursor: pointer;
    box-shadow: 0 0 10px #00c853;
    transition: background 0.2s ease-in-out;
  }

  .play-button:hover {
    background-color: #00e676;
  }

  .footer {
    font-size: 0.8em;
    color: #ccc;
    margin-top: 30px;
  }
</style>

<div class="overlay">
  <div class="title">WEBCRAFT</div>

  <div class="content-box">
    <p>Select a version and click Play to launch:</p>
  </div>

  <div class="play-bar">
    <div class="version-selector">
      <select id="versionSelect">
        <option value="https://eaglercraft.com/mc/1.5.2">1.5.2</option>
        <option value="https://eaglercraft.com/mc/1.8.8">1.8.8</option>
        <option value="https://eaglercraft.com/mc/1.12.2">1.12.2</option>
      </select>
    </div>
    <button class="play-button" onclick="launchGame()">PLAY</button>
  </div>

  <div class="footer">
    &copy; 2025 Webcraft. Not affiliated with Mojang or Microsoft.
  </div>
</div>

<script>
  function launchGame() {
    const selectedURL = document.getElementById('versionSelect').value;
    window.open(selectedURL, '_blank');
  }
</script>
