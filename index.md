4
---
layout: default
---

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>WEBCRAFT Launcher</title>
  <link href="https://fonts.cdnfonts.com/css/minecraft-4" rel="stylesheet">
  <style>
    body {
      margin: 0;
      padding: 0;
      background-image: url('https://cdn.mos.cms.futurecdn.net/qHFzGKFBz7kvxiVyjoe6JJ.jpg');
      background-size: cover;
      background-position: center;
      font-family: 'Minecraft', sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .launcher {
      background: rgba(0, 0, 0, 0.7);
      padding: 60px;
      border-radius: 15px;
      text-align: center;
      box-shadow: 0 0 20px black;
      width: 400px;
    }

    .logo {
      font-size: 48px;
      color: #00ff00;
      margin-bottom: 30px;
      text-shadow: 2px 2px #003300;
    }

    .play-btn {
      background-color: #00aa00;
      color: white;
      border: none;
      font-size: 24px;
      padding: 15px 50px;
      border-radius: 10px;
      cursor: pointer;
      font-family: 'Minecraft', sans-serif;
      box-shadow: 3px 3px #003300;
    }

    .play-btn:hover {
      background-color: #00cc00;
    }
  </style>
</head>
<body>
  <div class="launcher">
    <div class="logo">WEBCRAFT</div>
    <button class="play-btn" onclick="window.location.href='YOUR_GAME_SESSION_URL';">Play</button>
  </div>
</body>
</html>