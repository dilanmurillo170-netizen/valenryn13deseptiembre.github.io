<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>¿Quieres ser mi novia? ❤️‍🩹</title>
  <style>
    /* Estilos generales */
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
      padding: 15px;
      box-sizing: border-box;
    }

    .container {
      width: 100%;
      max-width: 650px; /* óptimo para iPhone 7 Plus y 13 */
    }

    /* Galería de imágenes */
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(130px, 1fr));
      gap: 12px;
      margin-bottom: 20px;
    }

    .gallery img {
      width: 100%;
      height: auto;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.3);
      cursor: pointer;
      transition: transform 0.3s;
    }

    .gallery img:hover {
      transform: scale(1.05);
    }

    /* Declaración */
    .declaration {
      background: rgba(255, 255, 255, 0.2);
      padding: 18px;
      border-radius: 15px;
      box-shadow: 0 6px 18px rgba(0,0,0,0.3);
      margin-bottom: 20px;
    }

    .declaration h1 {
      font-size: 1.9rem;
      margin-bottom: 10px;
      color: #fff;
    }

    .declaration p {
      font-size: 1rem;
      margin-bottom: 15px;
      line-height: 1.4;
    }

    .question {
      font-size: 1.3rem;
      font-weight: bold;
      margin-bottom: 12px;
    }

    /* Botones */
    .buttons {
      display: flex;
      gap: 12px;
      justify-content: center;
      flex-wrap: wrap;
    }

    .btn {
      background: #fff;
      color: #ff69b4;
      border: none;
      padding: 10px 15px;
      border-radius: 10px;
      font-size: 1rem;
      cursor: pointer;
      transition: 0.3s;
      flex: 1 1 45%;
      max-width: 220px;
    }

    .btn:hover {
      background: #ff69b4;
      color: #fff;
    }

    /* Modal de texto */
    .modal-backdrop {
      position: fixed;
      inset: 0;
      background: rgba(0,0,0,0.6);
      display: flex;
      align-items: center;
      justify-content: center;
      opacity: 0;
      pointer-events: none;
      transition: opacity 0.3s;
      z-index: 1000;
    }

    .modal-backdrop.show {
      opacity: 1;
      pointer-events: auto;<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>¿Quieres ser mi novia? ❤️‍🩹</title>
  <style>
    /* Estilos generales */
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #ffb6c1, #ff69b4);
      color: #fff;
      text-align: center;
      padding: 15px;
      box-sizing: border-box;
    }

    .container {
      width: 100%;
      max-width: 650px;
      margin: 0 auto;
    }

    /* Galería de imágenes */
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(130px, 1fr));
      gap: 12px;
      margin-bottom: 20px;
    }

    .gallery img {
      width: 100%;
      height: auto;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.3);
      cursor: pointer;
      transition: transform 0.3s;
    }

    .gallery img:hover {
      transform: scale(1.05);
    }

    /* Declaración */
    .declaration {
      background: rgba(255, 255, 255, 0.2);
      padding: 18px;
      border-radius: 15px;
      box-shadow: 0 6px 18px rgba(0,0,0,0.3);
      margin-bottom: 20px;
    }

    .declaration h1 {
      font-size: 1.9rem;
      margin-bottom: 10px;
      color: #fff;
    }

    .declaration p {
      font-size: 1rem;
      margin-bottom: 15px;
      line-height: 1.4;
      text-align: justify;
    }

    .question {
      font-size: 1.3rem;
      font-weight: bold;
      margin-bottom: 12px;
    }

    /* Botones */
    .buttons {
      display: flex;
      gap: 12px;
      justify-content: center;
      flex-wrap: wrap;
    }

    .btn {
      background: #fff;
      color: #ff69b4;
      border: none;
      padding: 10px 15px;
      border-radius: 10px;
      font-size: 1rem;
      cursor: pointer;
      transition: 0.3s;
      flex: 1 1 45%;
      max-width: 220px;
      text-decoration: none; /* para links de WhatsApp */
      display: inline-block;
    }

    .btn:hover {
      background: #ff69b4;
      color: #fff;
    }

    /* Modal de texto */
    .modal-backdrop {
      position: fixed;
      inset: 0;
      background: rgba(0,0,0,0.6);
      display: flex;
      align-items: center;
      justify-content: center;
      opacity: 0;
      pointer-events: none;
      transition: opacity 0.3s;
      z-index: 1000;
    }

    .modal-backdrop.show {
      opacity: 1;
      pointer-events: auto;
    }

    .modal {
      background: #fff;
      color: #333;
      padding: 18px;
      border-radius: 12px;
      max-width: 90%;
      text-align: left;
      box-shadow: 0 6px 20px rgba(0,0,0,0.4);
      position: relative;
    }

    .modal h2 {
      margin-top: 0;
      color: #ff69b4;
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
      max-width: 95%;
      max-height: 90%;
      border-radius: 12px;
      box-shadow: 0 8px 24px rgba(0,0,0,0.5);
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

    /* Media queries móviles */
    @media (max-width: 480px) {
      .declaration h1 { font-size: 1.5rem; }
      .declaration p { font-size: 0.95rem; }
      .question { font-size: 1.1rem; }
      .btn { flex: 1 1 100%; max-width: 100%; }
      .gallery { grid-template-columns: 1fr; gap: 8px; }
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

  <!-- Modal texto (opcional, se puede quitar si solo quieres WhatsApp) -->
  <div id="modalBackdrop" class="modal-backdrop">
    <div class="modal">
      <h2>Gracias por decir que sí ❤️‍🩹</h2>
      <p>
        Gracias por decir que sí.  
        Llevaba estos 3 meses contigo esperando a ser tu novio. Perdóname por haberte hecho enojar tantas veces y por todas esas malas palabras; sé que estuvo muy mal mío, pero de igual manera te amo y no quiero perderte.
      </p>
    </div>
  </div>

  <!-- Visor de imágenes -->
  <div id="imageViewer" class="image-viewer">
    <span class="close-img" onclick="closeImage()">&times;</span>
    <img id="viewerImg" src="" alt="Foto ampliada">
  </div>

  <script>
    const backdrop = document.getElementById('modalBackdrop');
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
      if (e.target === viewer) closeImage();
    });
  </script>
</body>
</html>
