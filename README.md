Портфолио


<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Видео с Google Drive</title>
  <style>
    body {
      margin: 0;
      background-color: #0e0e0e;
      color: white;
      font-family: sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
    }

    .video-container {
      position: relative;
      width: 90%;
      max-width: 960px;
      aspect-ratio: 16 / 9;
      box-shadow: 0 0 25px rgba(0, 0, 0, 0.7);
      border-radius: 12px;
      overflow: hidden;
    }

    video {
      width: 100%;
      height: 100%;
      border-radius: 12px;
      background: #000;
      object-fit: cover;
    }

    @media (max-width: 600px) {
      .video-container {
        width: 100%;
        border-radius: 0;
      }
    }
  </style>
</head>
<body>
  <div class="video-container">
    <video controls preload="metadata">
      <source src="https://drive.google.com/uc?export=download&id=1URJvP9RENQRd1Yp3LP8PciLKPxaL31hO" type="video/mp4">
      Ваш браузер не поддерживает воспроизведение видео.
    </video>
  </div>
</body>
</html>
