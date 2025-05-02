---
layout: default
title: Webcraft Launcher
---

<style>
  body {
    margin: 0;
    padding: 0;
    background: url('https://feedback.minecraft.net/hc/article_attachments/35363543357965') no-repeat center center fixed;
    background-size: cover;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    color: #ffffff;
  }

  .overlay {
    background-color: rgba(0, 0, 0, 0.75);
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 40px 20px;
  }

  .launcher-box {
    background-color: #2d2d2d;
    border-radius: 10px;
    padding: 30px;
    max-width: 500px;
    width: 100%;
    text-align: center;
    box-shadow: 0 0 25px rgba(0, 0, 0, 0.8);
  }

  .launcher-box h1 {
    margin-bottom: 20px;
    font-size: 2em;
    color: #00c853;
  }

  .launcher-box p {
    margin-bottom: 30px;
  }

  .launcher-box a {
    display: block;
    background-color: #00c853;
    color: #000;
    text-decoration: none;
    margin: 10px 0;
    padding: 12px;
    border-radius: 5px;
    font-weight: bold;
    transition: background 0.3s;
  }

  .launcher-box a:hover {
    background-color: #00e676;
  }

  .footer {
    margin-top: 40px;
    font-size: 0.8em;
    color: #ccc;
    text-align: center;
  }
</style>

<div class="overlay">
  <div class="launcher-box">
    <h1>Webcraft Launcher</h1>
    <p>Choose your version:</p>
    <a href="https://eaglercraft.com/mc/1.5.2" target="_blank">Play 1.5.2</a>
    <a href="https://eaglercraft.com/mc/1.8.8" target="_blank">Play 1.8.8</a>
    <a href="https://eaglercraft.com/mc/1.12.2" target="_blank">Play 1.12.2</a>
  </div>
  <div class="footer">
    &copy; 2025 Webcraft. Not affiliated with Mojang or Microsoft.
  </div>
</div>
