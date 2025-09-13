
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>¿Quieres ser mi novia? ❤️‍🩹</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #ffb6c1, #ff69b4);
      color: #fff;
      text-align: center;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      padding: 20px;
    }

    .container {
      max-width: 900px;
      width: 100%;
    }

    .gallery {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 15px;
      margin-bottom: 25px;
    }

    .gallery img {
      max-width: 100%;
      height: auto;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.3);
      cursor: pointer;
      transition: transform 0.3s;
    }

    .gallery img:hover {
      transform: scale(1.05);
    }

    /* 📌 Recuadro para el texto */
    .declaration {
      background: rgba(255, 255, 255, 0.2); /* semi-transparente */
      padding: 20px;
      border-radius: 15px;
      box-shadow: 0 6px 18px rgba(0,0,0,0.3);
      margin-bottom: 20px;
    }

    .declaration h1 {
      font-size: 2rem;
      margin-bottom: 10px;
      color: #fff;
    }

    .declaration p {
      font-size: 1.1rem;
      margin-bottom: 20px;
      line-height: 1.5;
    }

    .question {
      font-size: 1.4rem;
      font-weight: bold;
      margin-bottom: 15px;
    }

    .buttons {
      display: flex;
      gap: 15px;
      justify-content: center;
      flex-wrap: wrap;
    }

    .btn {
      background: #fff;
      color: #ff69b4;
      border: none;
      padding: 10px 20px;
      border-radius: 10px;
      font-size: 1rem;
      cursor: pointer;
      transition: 0.3s;
    }

    .btn:hover {
      background: #ff69b4;
      color: #fff;
    }

    /* Modal de imagen */
    .image-viewer {
      position: fixed;
      inset: 0;
      background: rgba(0,0,0,0.85);
      display: flex;
      align-items: center;
      justify-content: center;
      opacity: 0;
      pointer-events: none;
      transition: opacity 0.3s;
      z-index: 2000;
    }
    .image-viewer.show {
      opacity: 1;
      pointer-events: auto;
    }
    .image-viewer img {
      max-width: 90%;
      max-height: 90%;
      border-radius: 12px;
      box-shadow: 0 8px 24px rgba(0,0,0,0.5);
    }
    .close-img {
      position: absolute;
      top: 20px;
      right: 30px;
      font-size: 2rem;
      color: #fff;
      cursor: pointer;
      font-weight: bold;
    }

    /* Responsive */
    @media (max-width: 600px) {
      .declaration h1 { font-size: 1.5rem; }
      .question { font-size: 1.1rem; }
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="gallery">
      <img src="https://i.ibb.co/fJQcD85/2.jpg" alt="Foto 1">
      <img src="https://i.ibb.co/xKhHywX0/2.jpg" alt="Foto 3">
      <img src="https://i.ibb.co/JLKYrV2/2.jpg" alt="Foto 4">
      <img src="https://i.ibb.co/7xmHxqZ8/2.jpg" alt="Foto 5">
    </div>

    <!-- 📌 Texto en recuadro -->
    <div class="declaration">
      <h1>Para Mi Morochita</h1>
      <p>La verdad ya no me aguanto más, desde hace 3 meses que hablamos cada día me gustas más y no puedo seguir logrando que tú no me quieras; por esto te hice todo esto, para que veas que de verdad te quiero y te amo. No dejes de quererme. ❤️‍🩹</p>

      <div class="question">¿Quieres ser mi novia?</div>

      <div class="buttons">
        <button class="btn" onclick="window.location.href='https://wa.me/573146553778?text=Si+quiero+ser+tu+novia+❤️'">Sí ❤️‍🩹</button>
        <button class="btn" onclick="window.location.href='https://wa.me/573146553778?text=Obviamente+si+quiero+ser+tu+novia+😍'">Obviamente sí 😍</button>
      </div>
    </div>
  </div>

  <!-- Visor de imágenes -->
  <div id="imageViewer" class="image-viewer">
    <span class="close-img" onclick="closeImage()">&times;</span>
    <img id="viewerImg" src="" alt="Foto ampliada">
  </div>

  <script>
    const viewer = document.getElementById('imageViewer');
    const viewerImg = document.getElementById('viewerImg');

    // Visor de imágenes
    document.querySelectorAll('.gallery img').forEach(img => {
      img.addEventListener('click', () => {
        viewerImg.src = img.src;
        viewer.classList.add('show');
      });
    });

    function closeImage() {
      viewer.classList.remove('show');
      viewerImg.src = "";
    }

    viewer.addEventListener('click', (e) => {
      if (e.target === viewer) closeImage();
    });
  </script>
</body>
</html>

