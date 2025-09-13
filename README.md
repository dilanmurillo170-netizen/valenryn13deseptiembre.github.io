<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <!-- Ajuste de escala para que se vea más pequeño en iPhone 7 -->
  <meta name="viewport" content="width=375, initial-scale=0.85, maximum-scale=1.0, user-scalable=no">
  <title>¿Quieres ser mi novia? ❤️‍🩹</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #ffb6c1, #ff69b4);
      color: #fff;
      text-align: center;
    }

    body {
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
    }

    .container {
      width: 100%;
      max-width: 600px; /* más pequeño que iPhone 13 */
      padding: 15px;
      box-sizing: border-box;
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
      gap: 10px;
      margin-bottom: 20px;
    }

    .gallery img {
      width: 100%;
      border-radius: 12px;
      cursor: pointer;
      transition: transform 0.3s;
    }

    .gallery img:hover { transform: scale(1.05); }

    .declaration {
      background: rgba(255, 255, 255, 0.2);
      padding: 15px;
      border-radius: 15px;
      margin-bottom: 20px;
    }

    .declaration h1 { font-size: 1.6rem; margin-bottom: 10px; }
    .declaration p { font-size: 0.95rem; margin-bottom: 15px; line-height: 1.4; text-align: justify; }
    .question { font-size: 1.2rem; margin-bottom: 12px; font-weight: bold; }

    .buttons {
      display: flex;
      gap: 10px;
      justify-content: center;
      flex-wrap: wrap;
    }

    .btn {
      background: #fff;
      color: #ff69b4;
      text-decoration: none;
      padding: 10px;
      border-radius: 10px;
      font-size: 0.95rem;
      flex: 1 1 45%;
      max-width: 180px;
      display: inline-block;
      transition: 0.3s;
    }

    .btn:hover {
      background: #ff69b4;
      color: #fff;
    }

    /* Modal imágenes */
    .image-viewer {
      position: fixed;
      inset: 0;
      background: rgba(0,0,0,0.85);
      display: flex;
      justify-content: center;
      align-items: center;
      opacity: 0;
      pointer-events: none;
      transition: opacity 0.3s;
      z-index: 2000;
    }

    .image-viewer.show { opacity: 1; pointer-events: auto; }

    .image-viewer img {
      max-width: 90%;
      max-height: 85%;
      border-radius: 12px;
    }

    .close-img {
      position: absolute;
      top: 15px;
      right: 20px;
      font-size: 2rem;
      color: #fff;
      cursor: pointer;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="gallery">
      <img src="https://i.ibb.co/fJQcD85/2.jpg" alt="Foto 1">
      <img src="https://i.ibb.co/jPBwRkzM/2.jpg" alt="Foto 2">
      <img src="https://i.ibb.co/JLKYrV2/2.jpg" alt="Foto 3">
      <img src="https://i.ibb.co/7xmHxqZ8/2.jpg" alt="Foto 4">
    </div>

    <div class="declaration">
      <h1>Para Mi Morochita</h1>
      <p>La verdad ya no me aguanto más, desde hace 3 meses que hablamos cada día me gustas más y no puedo seguir logrando que tú no me quieras, por esto te hice todo esto, sé que estuvo muy mal mío, por eso quiero que me perdones. Yo sé que no soy perfecto, soy humano y cometo errores, pero trato de mejorar para ser el hombre que te ame y no te abandone. ❤️‍🩹</p>

      <div class="question">¿Quieres ser mi novia?</div>

      <div class="buttons">
        <a class="btn" href="https://wa.me/573146553778?text=Hola,%20acepto%20ser%20tu%20novia%20❤️" target="_blank">Sí ❤️‍🩹</a>
        <a class="btn" href="https://wa.me/573146553778?text=Hola,%20obviamente%20sí%20😍" target="_blank">Obviamente sí 😍</a>
      </div>
    </div>
  </div>

  <div id="imageViewer" class="image-viewer">
    <span class="close-img" onclick="closeImage()">&times;</span>
    <img id="viewerImg" src="" alt="Foto ampliada">
  </div>

  <script>
    const viewer = document.getElementById('imageViewer');
    const viewerImg = document.getElementById('viewerImg');

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
      if(e.target === viewer) closeImage();
    });
  </script>
</body>
</html>

