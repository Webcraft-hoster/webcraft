---
layout: default
title: Webcraft Launcher
---

<link href="https://fonts.cdnfonts.com/css/minecraftia" rel="stylesheet">

<style>
  html, body {
    margin: 0;
    padding: 0;
    overflow: hidden;
    height: 100%;
    font-family: 'Minecraftia', monospace;
    background: url('https://feedback.minecraft.net/hc/article_attachments/35363543357965') no-repeat center center fixed;
    background-size: cover;
    color: #fff;
  }

  .overlay {
    position: relative;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
  }

  .title {
    font-size: 3em;
    color: gray;
    margin-top: 40px;
    text-shadow: 2px 2px #000;
  }

  .play-bar {
    background-color: #1e1e1e;
    width: 100%;
    padding: 10px 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    position: fixed;
    bottom: 0;
    left: 0;
    border-top: 2px solid #444;
  }

  .version-selector {
    position: absolute;
    left: 20px;
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
</style>

<div class="overlay">
  <div class="title">WEBCRAFT</div>

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
</div>

<script>
  function launchGame() {
    const selectedURL = document.getElementById('versionSelect').value;
    window.open(selectedURL, '_blank');
  }
</script>
