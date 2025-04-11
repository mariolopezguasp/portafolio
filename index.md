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
<div style="max-width: 900px; margin: 0 auto; padding: 30px; font-family: Arial, sans-serif;">

  <!-- Header completo con foto a la izquierda y datos a la derecha -->
  <div style="display: flex; align-items: center; gap: 30px; margin-bottom: 40px;">
    <!-- Imagen -->
    <img src="assets/fotocarnetmario.jfif" alt="Foto de Mario" style="width: 120px; height: 120px; border-radius: 10%; object-fit: cover; border: 2px solid #3498db;">
    <!-- Información: nombre, título y botones -->
    <div style="display: flex; flex-direction: column; gap: 12px;">
      <!-- Nombre y título -->
      <div>
        <h1 style="color: #2c3e50; font-size: 2.2em; margin: 0;">Mario López Guasp</h1>
        <h2 style="color: #3498db; font-weight: 300; margin: 0;">DATA SCIENTIST</h2>
      </div>
      <!-- Botones de contacto -->
      <div style="display: flex; flex-wrap: wrap; gap: 10px;">
        <a href="mailto:mariolopezguasp@gmail.com" style="text-decoration: none;">
          <div style="display: flex; align-items: center; gap: 8px; background-color: #fff5f5; padding: 6px 10px; border-radius: 6px; border: 1px solid #3498db;">
            <span style="color: #000000;">mariolopezguasp@gmail.com</span>
          </div>
        </a>
        <a href="assets/CurriculumMario.pdf" target="_blank" style="text-decoration: none;">
          <div style="display: flex; align-items: center; gap: 8px; background-color: #f0fff4; padding: 6px 10px; border-radius: 6px; border: 1px solid #3498db;">
            <span style="color: #0077b5; font-weight: 500;">📄 CV</span>
          </div>
        </a>
        <a href="https://www.linkedin.com/in/mario-l%C3%B3pez-guasp-56b462225/" target="_blank" style="text-decoration: none;">
          <div style="display: flex; align-items: center; gap: 8px; background-color: #eaf4fb; padding: 6px 10px; border-radius: 6px; border: 1px solid #3498db;">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linkedin/linkedin-original.svg" alt="LinkedIn" style="width: 20px; height: 20px;">
            <span style="color: #0077b5;">LinkedIn</span>
          </div>
        </a>
        <a href="https://github.com/mariolopezguasp" target="_blank" style="text-decoration: none;">
          <div style="display: flex; align-items: center; gap: 8px; background-color: #f5f5f5; padding: 6px 10px; border-radius: 6px; border: 1px solid #3498db;">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="GitHub" style="width: 20px; height: 20px;">
            <span style="color: #0077b5;">GitHub</span>
          </div>
        </a>
      </div>
    </div>
  </div>

  <!-- Sección Sobre mí -->
  <div style="margin-bottom: 40px;">
    <h3 style="color: #2c3e50; border-bottom: 2px solid #3498db; padding-bottom: 5px;">Sobre mi</h3>
    <p style="line-height: 1.6; margin: 0;">Soy un científico de datos en proceso de finalizar mis estudios de Ciencia de Datos en la Universidad de Valencia. Estoy muy motivado a desarrollar mis habilidades y conocimientos en el mundo laboral. Tengo una actitud proactiva que hará que mi trabajo se complemente con la visión y objetivos de la empresa.</p>
  </div>


<!-- Añadir Devicon -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/devicons/devicon@v2.15.1/devicon.min.css">

<!-- Sección Tecnologías -->
<div style="margin-bottom: 40px;">
  <h3 style="color: #2c3e50; border-bottom: 2px solid #3498db; padding-bottom: 5px;">Tecnologías</h3>
  <div style="display: flex; flex-wrap: wrap; gap: 10px;">
    <span style="background: #e0f7fa; padding: 5px 10px; border-radius: 4px; display: flex; align-items: center;">
      <i class="devicon-python-plain" style="font-size: 30px; margin-right: 8px;"></i> Python
    </span>
    <span style="background: #e0f7fa; padding: 5px 10px; border-radius: 4px; display: flex; align-items: center;">
      <i class="devicon-r-plain" style="font-size: 30px; margin-right: 8px;"></i> R
    </span>
    <span style="background: #e0f7fa; padding: 5px 10px; border-radius: 4px; display: flex; align-items: center;">
      <i class="devicon-mysql-plain" style="font-size: 30px; margin-right: 8px;"></i> SQL
    </span>
    <span style="background: #e0f7fa; padding: 5px 10px; border-radius: 4px; display: flex; align-items: center;">
      <i class="devicon-tensorflow-original" style="font-size: 30px; margin-right: 8px;"></i> TensorFlow
    </span>
  </div>
</div>

<!-- Sección Proyectos -->
<div style="margin-bottom: 40px;">
  <h3 style="color: #2c3e50; border-bottom: 2px solid #3498db; padding-bottom: 5px;">Proyectos</h3>
  <div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 20px; margin-bottom: 15px;">
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
    <a href="#img1"><img src="assets/verdep.PNG" alt="Web ValenciaVerde" class="zoomable" style="width: 280px; border-radius: 10px; object-fit: cover;"></a>
  </div>

  <!-- Lightbox para ver en grande -->
  <div id="img1" class="lightbox">
    <a href="#" class="lightbox-close">&times;</a>
    <img src="assets/verdep.PNG" alt="Web ValenciaVerde Ampliada">
  </div>
</div>

  <!-- Sección Formación -->
  <div style="margin-bottom: 40px;">
    <h3 style="color: #2c3e50; border-bottom: 2px solid #3498db; padding-bottom: 5px;">Formación</h3>
    <div style="margin-bottom: 15px;">
      <h4 style="margin-bottom: 5px;">Ciencia de Datos | 2022 - 2026</h4>
      <p style="margin: 0; line-height: 1.6;">Universidad de Valencia</p>
    </div>
  </div>

<!-- Sección Otros trabajos -->
<div style="margin-bottom: 40px;">
  <h3 style="color: #2c3e50; border-bottom: 2px solid #3498db; padding-bottom: 5px;">Otros trabajos realizados</h3>
     <!-- Ejemplo modificado con zoom y ampliación -->
  <div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 20px; margin-bottom: 15px;">
    <div style="flex: 1;">
      <h4 style="margin-bottom: 5px;">Análisis exploratorio completo sobre un dataset de vino</h4>
      <p style="margin: 0; line-height: 1.6;">Procesos de ETL, extracción de características y visualización sobre los datos del vino.</p>
      <a href="https://github.com/mariolopezguasp/Vino" target="_blank" style="text-decoration: none;">
        <div style="display: inline-flex; align-items: center; gap: 8px; background-color: #f5f5f5; padding: 5px 10px; border-radius: 6px; border: 1px solid #3498db; margin-top: 5px;">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="GitHub" style="width: 18px; height: 18px;">
        </div>
      </a>
    </div>
    <!-- Imagen con zoom y lightbox -->
    <a href="#img2"><img src="assets/vino.PNG" alt="Web ValenciaVerde" class="zoomable" style="width: 220px; border-radius: 10px; object-fit: cover;"></a>
  </div>

  <!-- Lightbox para ver en grande -->
  <div id="img2" class="lightbox">
    <a href="#" class="lightbox-close">&times;</a>
    <img src="assets/vino.PNG" alt="Web ValenciaVerde Ampliada">
  </div>

  <div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 20px; margin-bottom: 15px;">
    <div style="flex: 1;">
      <h4 style="margin-bottom: 5px;">Predicción del precio de vivienda en Florida</h4>
      <p style="margin: 0; line-height: 1.6;">Entrenamiento de un modelo de regresión para predecir el precio de la vivienda en Florida.</p>
      <a href="https://github.com/mariolopezguasp/CasasCalifornia" target="_blank" style="text-decoration: none;">
        <div style="display: inline-flex; align-items: center; gap: 8px; background-color: #f5f5f5; padding: 5px 10px; border-radius: 6px; border: 1px solid #3498db; margin-top: 5px;">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="GitHub" style="width: 18px; height: 18px;">
        </div>
      </a>
    </div>
    <!-- Imagen con zoom y lightbox -->
    <a href="#img3"><img src="assets/RF.PNG" alt="Web ValenciaVerde" class="zoomable" style="width: 220px; border-radius: 10px; object-fit: cover;"></a>
  </div>

   <!-- Lightbox para ver en grande -->
  <div id="img3" class="lightbox">
    <a href="#" class="lightbox-close">&times;</a>
    <img src="assets/RF.PNG" alt="Web ValenciaVerde Ampliada">
  </div>

  <div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 20px; margin-bottom: 15px;">
    <div style="flex: 1;">
      <h4 style="margin-bottom: 5px;">Agrupamiento de sonidos</h4>
      <p style="margin: 0; line-height: 1.6;">Análisis no supervisado para agrupar distintos sonidos según sus características acústicas.</p>
      <a href="https://github.com/mariolopezguasp/AgrupamientoSonidos" target="_blank" style="text-decoration: none;">
        <div style="display: inline-flex; align-items: center; gap: 8px; background-color: #f5f5f5; padding: 5px 10px; border-radius: 6px; border: 1px solid #3498db; margin-top: 5px;">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="GitHub" style="width: 18px; height: 18px;">
        </div>
      </a>
    </div>
    <!-- Imagen con zoom y lightbox -->
    <a href="#img4"><img src="assets//cluster.PNG" alt="Web ValenciaVerde" class="zoomable" style="width: 220px; border-radius: 10px; object-fit: cover;"></a>
  </div>

   <!-- Lightbox para ver en grande -->
  <div id="img4" class="lightbox">
    <a href="#" class="lightbox-close">&times;</a>
    <img src="assets//cluster.PNG" alt="Web ValenciaVerde Ampliada">
  </div>

  <!-- Footer con botones de contacto -->
  <div style="text-align: center; margin-top: 20px;">
    <div style="display: flex; justify-content: center; flex-wrap: wrap; gap: 10px; margin-top: 20px;">
      <a href="mailto:mariolopezguasp@gmail.com" style="text-decoration: none;">
        <div style="display: flex; align-items: center; gap: 8px; background-color: #fff5f5; padding: 6px 10px; border-radius: 6px; border: 1px solid #3498db;">
          <span style="color: #000000;">mariolopezguasp@gmail.com</span>
        </div>
      </a>
      <a href="assets/CurriculumMario.pdf" target="_blank" style="text-decoration: none;">
        <div style="display: flex; align-items: center; gap: 8px; background-color: #f0fff4; padding: 6px 10px; border-radius: 6px; border: 1px solid #3498db;">
          <span style="color: #0077b5; font-weight: 500;">📄 CV</span>
        </div>
      </a>
      <a href="https://www.linkedin.com/in/mario-l%C3%B3pez-guasp-56b462225/" target="_blank" style="text-decoration: none;">
        <div style="display: flex; align-items: center; gap: 8px; background-color: #eaf4fb; padding: 6px 10px; border-radius: 6px; border: 1px solid #3498db;">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linkedin/linkedin-original.svg" alt="LinkedIn" style="width: 20px; height: 20px;">
          <span style="color: #0077b5;">LinkedIn</span>
        </div>
      </a>
      <a href="https://github.com/mariolopezguasp" target="_blank" style="text-decoration: none;">
        <div style="display: flex; align-items: center; gap: 8px; background-color: #f5f5f5; padding: 6px 10px; border-radius: 6px; border: 1px solid #3498db;">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="GitHub" style="width: 20px; height: 20px;">
          <span style="color: #0077b5;">GitHub</span>
        </div>
      </a>
    </div>
  </div>

</div>
