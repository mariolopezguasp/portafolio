<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Mario López Guasp - Portfolio</title>
  <style>
    /* Estilos base */
    body {
      font-family: Arial, sans-serif;
    }
    img.zoomable {
      transition: transform 0.3s ease;
      cursor: zoom-in;
    }
    img.zoomable:hover {
      transform: scale(1.05);
    }
    /* Lightbox (pantalla completa al hacer clic) */
    .lightbox {
      display: none;
      position: fixed;
      z-index: 1000;
      top: 0; left: 0;
      width: 100vw;
      height: 100vh;
      background-color: rgba(0,0,0,0.8);
      justify-content: center;
      align-items: center;
    }
    .lightbox img {
      max-width: 90%;
      max-height: 90%;
      border-radius: 10px;
      box-shadow: 0 0 15px rgba(0,0,0,0.5);
    }
    .lightbox:target {
      display: flex;
    }
    /* Botón de cerrar */
    .lightbox-close {
      position: absolute;
      top: 20px;
      right: 30px;
      font-size: 40px;
      color: white;
      text-decoration: none;
      font-weight: bold;
    }
    .lightbox-close:hover {
      color: #ddd;
    }
  </style>
</head>
<body>

<!-- CONTENEDOR PRINCIPAL -->
<div style="max-width: 900px; margin: 0 auto; padding: 30px;">

  <!-- ... TODO TU CONTENIDO DE ANTES SE MANTIENE IGUAL ... -->

  <!-- Ejemplo modificado con zoom y ampliación -->
  <div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 20px; margin-bottom: 15px;">
    <div style="flex: 1;">
      <h4 style="margin-bottom: 5px;">Web dinámica sobre datos medioambientales georreferenciados</h4>
      <p style="margin: 0; line-height: 1.6;">Análisis y visualización de datos relativos a la contaminación atmosférica y zonas verdes con tal de comprender los motivos que han llevado a Valencia a ser elegida Capital Verde Europea 2024.</p>
      <a href="https://github.com/mariolopezguasp/ValenciaVerde" target="_blank" style="text-decoration: none;">
        <div style="display: inline-flex; align-items: center; gap: 8px; background-color: #f5f5f5; padding: 5px 10px; border-radius: 6px; border: 1px solid #3498db; margin-top: 5px;">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="GitHub" style="width: 18px; height: 18px;">
        </div>
      </a>
    </div>
    <!-- Imagen con zoom y lightbox -->
    <a href="#img1"><img src="assets/verdep.PNG" alt="Web ValenciaVerde" class="zoomable" style="width: 260px; border-radius: 10px; object-fit: cover;"></a>
  </div>

  <!-- Lightbox para ver en grande -->
  <div id="img1" class="lightbox">
    <a href="#" class="lightbox-close">&times;</a>
    <img src="assets/verdep.PNG" alt="Web ValenciaVerde Ampliada">
  </div>

  <!-- Puedes repetir este patrón para todas las imágenes del portfolio -->
  <!-- Otro ejemplo -->
  <div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 20px; margin-bottom: 15px;">
    <div style="flex: 1;">
      <h4 style="margin-bottom: 5px;">Análisis de Vino</h4>
      <p style="margin: 0 0 8px 0; line-height: 1.6;">Procesos de ETL, extracción de características y visualización sobre los datos del vino.</p>
      <a href="https://github.com/mariolopezguasp/Vino" target="_blank" style="text-decoration: none;">
        <div style="display: inline-flex; align-items: center; gap: 8px; background-color: #f5f5f5; padding: 5px 10px; border-radius: 6px; border: 1px solid #3498db; margin-top: 5px;">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="GitHub" style="width: 18px; height: 18px;">
        </div>
      </a>
    </div>
    <a href="#img2"><img src="assets/vino.PNG" alt="Análisis de Vino" class="zoomable" style="width: 250px; border-radius: 10px; object-fit: cover;"></a>
  </div>

  <div id="img2" class="lightbox">
    <a href="#" class="lightbox-close">&times;</a>
    <img src="assets/vino.PNG" alt="Análisis de Vino Ampliado">
  </div>

</div>

</body>
</html>
