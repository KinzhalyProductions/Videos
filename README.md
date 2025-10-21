<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Видео — Kinzhaly Productions</title>
  <style>
    :root { --bg:#0b0b0b; --card:#0f0f0f; --radius:12px; }
    body{
      margin:0;
      min-height:100vh;
      display:flex;
      align-items:center;
      justify-content:center;
      background:linear-gradient(180deg,var(--bg) 0%, #0f1720 100%);
      color:#fff;
      font-family:Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      padding:24px;
      box-sizing:border-box;
    }

    .wrap {
      width:100%;
      max-width:1100px;
      margin:0 auto;
    }

    .player-card{
      background:var(--card);
      border-radius:var(--radius);
      overflow:hidden;
      box-shadow: 0 10px 30px rgba(2,6,23,0.6);
    }

    /* Responsive 16:9 container for iframe */
    .video-embed {
      position:relative;
      width:100%;
      padding-top:56.25%; /* 16:9 */
      background:#000;
    }
    .video-embed iframe,
    .video-embed video {
      position:absolute;
      top:0; left:0;
      width:100%;
      height:100%;
      border:0;
    }

    .meta {
      padding:14px 18px;
      display:flex;
      gap:12px;
      align-items:center;
      justify-content:space-between;
    }
    .title { font-size:16px; font-weight:600; }
    .actions { font-size:14px; opacity:0.9; }

    .fallback {
      padding:14px 18px;
      background: linear-gradient(90deg, rgba(255,255,255,0.02), rgba(255,255,255,0.00));
      font-size:14px;
    }

    @media (max-width:600px){
      .meta { padding:10px; }
      .fallback { font-size:13px; padding:10px; }
    }
  </style>
</head>
<body>
  <div class="wrap">
    <div class="player-card" role="region" aria-label="Видео с Google Drive">
      <div class="video-embed">
        <!-- IFRAME: Google Drive preview -->
        <iframe
          src="https://drive.google.com/file/d/1URJvP9RENQRd1Yp3LP8PciLKPxaL31hO/preview"
          allow="autoplay; encrypted-media; fullscreen"
          allowfullscreen
          loading="lazy"
          title="Видео с Google Drive — Kinzhaly Productions"></iframe>
      </div>

      <div class="meta">
        <div class="title">Название видео (с Google Drive)</div>
        <div class="actions">Нажмите ▶ для воспроизведения • Поддержка fullscreen</div>
      </div>

      <div class="fallback">
        Если iframe не загружается — убедитесь, что файл общий (Доступ: «Любой по ссылке»). 
        Также можно скачать напрямую: 
        <a href="https://drive.google.com/uc?export=download&id=1URJvP9RENQRd1Yp3LP8PciLKPxaL31hO" target="_blank" rel="noopener" style="color:#9ad1ff;">скачать видео</a>.
      </div>
    </div>
  </div>
</body>
</html>
