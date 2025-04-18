# web-asal
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Impossible</title>
  <style>
    body {
      background: black;
      color: white;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
      text-align: center;
    }
    video {
      width: 200px;
      border-radius: 12px;
    }
    .play-button {
      margin-bottom: 10px;
      padding: 8px 16px;
      background: rgba(255,255,255,0.1);
      border: 1px solid white;
      border-radius: 8px;
      cursor: pointer;
    }
    .quote {
      margin-top: 20px;
      opacity: 0.8;
    }
  </style>
</head>
<body>

  <div class="play-button" onclick="playMusic()">Play Music</div>
  <video src="video.mp4" autoplay loop muted playsinline></video>
  <div class="quote">"Sometimes, silence says everything."</div>

  <audio id="bgMusic" src="music.mp3"></audio>
  <script>
    function playMusic() {
      document.getElementById('bgMusic').play();
    }
  </script>

</body>
</html>
