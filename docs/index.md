---
layout: default
title: Inicio
---

<section class="hero">

  <div class="hero-content">

    <div class="hero-image">
      <img src="{{ '/assets/img/profile.jpg' | relative_url }}" alt="Foto de perfil">
    </div>

    <div class="hero-text">
      <h1>Lucas Correa</h1>

      <p class="hero-role">
        Data Analyst · Visualización · Automatización
      </p>

    <p class="hero-description">
      Desarrollador de software y estudiante de ingeniería con experiencia en análisis de datos y visualización.
    </p>

      <!-- BOTONES -->
      <div class="hero-actions">
        <a href="#proyectos" class="btn primary">Ver Proyectos</a>
        <a href="{{ '/cv.pdf' | relative_url }}" class="btn secondary" target="_blank">Descargar CV</a>
      </div>

      <!-- LINKS -->
      <div class="hero-links">
        <a href="https://github.com/LucasVCorrea">GitHub</a>
        <a href="https://www.linkedin.com/in/lucas-correa-9b492b1a0/">LinkedIn</a>
        <a href="mailto:lucasvalentincorrea@gmail.com">Email</a>
      </div>

    </div>

  </div>

</section>

<section id="experiencia" class="section">
  <h2>Experiencia</h2>

  <div class="timeline">

    <div class="timeline-item">
      <h3>Analista de Datos</h3>
      <span>2024 - Actualidad</span>
      <p>Dashboards, análisis de datos en infracciones de tránsito y automatización de reportes.</p>
    </div>

    <div class="timeline-item">
      <h3>Desarrollador</h3>
      <span>2024 - Actualidad</span>
      <p>Desarrollo de sistemas de carga y registro.</p>
    </div>    
    <div class="timeline-item">
      <h3>Ayudante Universitario</h3>
      <span>2023 - 2026</span>
      <p>Ayudante en la asignatura ciencia de datos / organización de datos en FIUBA, Universidad de Buenos Aires</p>
    </div>
  </div>
  <h2>Estudios</h2>
  <div class="timeline">
    
    <div class="timeline-item">
      <h3>Universitario</h3>
      <span>2021 - Actualidad</span>
      <p>Estudiante de la Facultad de Ingeniería de la Universidad de Buenos Aires. Buenos Aires, Argentina</p>
      <h3>Extracurriculares</h3>
      <span>Ago.2022 - Ago.2022</span>
      <p>Full time intensive course in English as a Foreign Language studying at C1 Common European Framework level. Chester, England.</p>
      <span>2011 - 2019</span>
      <p>Estudiante de Inglés como lengua extranjera. Buenos Aires, Argentina</p>
    </div>
  </div>
</section>

<section id="skills" class="section">
  <h2>Skills</h2>

  <div>
    <span class="badge">Python</span>
    <span class="badge">Pandas</span>
    <span class="badge">Ciencias de la computación</span>
    <span class="badge">Streamlit</span>
    <span class="badge">Sklearn-ML</span>
    <span class="badge">SQL</span>
    <span class="badge">OOP</span>
  </div>
</section>

<section id="proyectos" class="section">
  <h2>Proyectos</h2>

  <div class="project-grid">

    <!-- PROYECTO TESSA -->
    <div class="project-card">
      <img src="{{ '/assets/img/Dashindex.png' | relative_url }}" alt="TESSA Dashboard">
      <div class="project-content">
        <h3>T.E.S.S.A</h3>
        <p>
          Plataforma de análisis y monitoreo de fiscalización de fotomultas, 
          con métricas operativas, visualizaciones dinámicas y seguimiento de rendimiento.
        </p>
        <div class="project-tech">
          <span>Python</span>
          <span>Streamlit</span>
          <span>Pandas</span>
          <span>Data Visualization</span>
        </div>
        <a href="{{ 'herramientas/tessa' | relative_url }}" class="btn primary">
          Ver detalle
        </a>
      </div>
    </div>

    <!-- OTRO PROYECTO -->
    <div class="project-card">
      <img src="{{ '/assets/img/webscrapcaptura.jpg' | relative_url }}" alt="Web Scraping">
      <div class="project-content">
        <h3>Web Scraping App</h3>
        <p>Sistema de extracción y procesamiento automático de datos desde múltiples fuentes.</p>
        <div class="project-tech">
          <span>Python</span>
          <span>BeautifulSoup</span>
          <span>Automation</span>
        </div>
        <a href="{{ 'herramientas/tai' | relative_url }}" class="btn primary">
          Ver detalle
        </a>
      </div>
    </div>
    <!-- OTRO PROYECTO -->
    <div class="project-card">
      <img src="{{ '/assets/img/Login.jpg' | relative_url }}" alt="Login">
      <div class="project-content">
        <h3>Actividad Municipal App</h3>
        <p>Dashboard interactivo sobre la actividad de fotomultas en un municipio. Desarrollado exclusivamente para la Universidad de La Matanza</p>
        <div class="project-tech">
          <span>Python</span>
          <span>Visualizacion</span>
          <span>Data Analytics</span>
        </div>
        <a href="{{ 'herramientas/berys' | relative_url }}" class="btn primary">
          Ver detalle
        </a>
      </div>
    </div>
  </div>
</section>
