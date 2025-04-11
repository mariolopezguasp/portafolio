<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Galería con Lightbox</title>
  <style>
    * {
      box-sizing: border-box;
    }
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }
    .gallery {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      padding: 20px;
      justify-content: center;
    }
    .gallery img {
      width: 200px;
      height: auto;
      cursor: pointer;
      border-radius: 8px;
      transition: transform 0.2s;
    }
    .gallery img:hover {
      transform: scale(1.05);
    }
    .lightbox {
      display: none;
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      background-color: rgba(0, 0, 0, 0.8);
      justify-content: center;
      align-items: center;
      z-index: 9999;
    }
    .lightbox img {
      max-width: 90%;
      max-height: 90%;
      border-radius: 8px;
    }
  </style>
</head>
<body>

  <div class="gallery">
    <img src="https://via.placeholder.com/600x400/0000FF/FFFFFF?text=Imagen+1" alt="Imagen 1" onclick="openLightbox(this.src)">
    <img src="https://via.placeholder.com/600x400/FF0000/FFFFFF?text=Imagen+2" alt="Imagen 2" onclick="openLightbox(this.src)">
    <img src="https://via.placeholder.com/600x400/00FF00/FFFFFF?text=Imagen+3" alt="Imagen 3" onclick="openLightbox(this.src)">
    <img src="https://via.placeholder.com/600x400/FFA500/FFFFFF?text=Imagen+4" alt="Imagen 4" onclick="openLightbox(this.src)">
  </div>

  <div class="lightbox" id="lightbox" onclick="closeLightbox(event)">
    <img id="lightbox-img" src="" alt="Imagen ampliada">
  </div>

  <script>
    function openLightbox(src) {
      const lightbox = document.getElementById('lightbox');
      const img = document.getElementById('lightbox-img');
      img.src = src;
      lightbox.style.display = 'flex';
    }

    function closeLightbox(event) {
      const lightbox = document.getElementById('lightbox');
      // Cierra el lightbox solo si se hace clic fuera de la imagen
      if (event.target === lightbox) {
        lightbox.style.display = 'none';
      }
    }
  </script>

</body>
</html>
