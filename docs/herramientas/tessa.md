---
layout: default
title: T.E.S.S.A
---

<div class="tool-hero">
  <h1>T.E.S.S.A</h1>
  <p class="tool-subtitle">
    Tablero de Estadística y Seguimiento de Actividad diseñado para optimizar la gestión sobre la fiscalización de fotomultas.
  </p>
  <p>
    Herramienta robusta y visualmente intuitiva desarrollada para la Gestión de Tránsito en la Universidad Nacional de La Matanza.
  </p>
</div>

---

## Descripción General

<div class="section-block">
Tessa centraliza la información clave para supervisores y fiscalizadores, ofreciendo una visión detallada de las operaciones diarias de fotomultas.
Facilita la toma de decisiones estratégicas y mejora la eficiencia operativa mediante métricas claras y visualizaciones dinámicas.
</div>

---

## Funcionalidades Principales

<div class="feature-grid">

<div class="feature-item">
<h3>Actividad por Fiscalizador</h3>
<p>Monitoreo de productividad individual y de equipo con datos precisos sobre desempeño.</p>
</div>

<div class="feature-item">
<h3>Actividad por Cliente</h3>
<p>Análisis de carga de trabajo y rendimiento asociado a cada cliente.</p>
</div>

<div class="feature-item">
<h3>Actividad por Cámara</h3>
<p>Métricas detalladas por cámara y tipo de dispositivo para optimización operativa.</p>
</div>

<div class="feature-item">
<h3>Actividad por Tipo de Revisión</h3>
<p>Clasificación de actividad según complejidad y tipo de revisión realizada.</p>
</div>

</div>

---

## Análisis de Datos y Visualización

<div class="section-block">
<h3>Métricas Comparativas</h3>
<p>Comparación entre períodos y objetivos para detectar desviaciones y oportunidades de mejora.</p>

<h3>Visualización Avanzada</h3>
<p>Gráficos interactivos y personalizables para interpretar grandes volúmenes de información.</p>

<h3>Valores Históricos</h3>
<p>Acceso a registros completos para análisis retrospectivo y detección de tendencias.</p>
</div>

---

## Perfil de Fiscalizador

<div class="section-block">
<h3>Actividad Diaria Personal</h3>
<p>Seguimiento detallado del progreso diario y volumen de revisiones.</p>

<h3>Comparativa de Rendimiento</h3>
<p>Comparación con promedio del equipo y líderes operativos.</p>

<h3>Desarrollo y Crecimiento</h3>
<p>Análisis de desempeño individual para mejora continua.</p>
</div>

---

## Vista del Producto

<div class="image-grid">
  <div class="image-card">
    <img src="{{ '/assets/img/Dashindex.png' | relative_url }}" alt="Dashboard principal">
    <h4>Dashboard Principal</h4>
  </div>
  <div class="image-card">
    <img src="{{ '/assets/img/Heatmap auditores.png' | relative_url }}" alt="Heatmap de Fiscalizadores">
    <h4>Heatmap de Fiscalizadores</h4>
  </div>
  <div class="image-card">
    <img src="{{ '/assets/img/Perfil Auditor.png' | relative_url }}" alt="Perfil fiscalizador">
    <h4>Perfil Fiscalizador</h4>
  </div>
  <div class="image-card">
    <img src="{{ '/assets/img/Info Camaras.png' | relative_url }}" alt="Información de Camaras">
    <h4>Información de Cámaras</h4>
  </div>
</div>

<!-- LIGHTBOX -->
<div id="lightbox" class="lightbox">
  <span class="close">&times;</span>
  <img class="lightbox-img">
</div>

<style>
.image-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
  margin-top: 20px;
}

.image-card {
  text-align: center;
}

.image-card img {
  width: 100%;
  cursor: pointer;
  border-radius: 8px;
  transition: transform 0.2s;
}

.image-card img:hover {
  transform: scale(1.03);
}

.image-card h4 {
  margin-top: 8px;
  font-weight: 500;
}

.lightbox {
  display: none;
  position: fixed;
  z-index: 999;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0,0,0,0.8);
  justify-content: center;
  align-items: center;
}

.lightbox-img {
  max-width: 90%;
  max-height: 90%;
}

.close {
  position: absolute;
  top: 20px;
  right: 30px;
  color: #fff;
  font-size: 40px;
  cursor: pointer;
}
</style>

<script>
document.addEventListener("DOMContentLoaded", function() {
  const images = document.querySelectorAll(".image-card img");
  const lightbox = document.getElementById("lightbox");
  const lightboxImg = document.querySelector(".lightbox-img");
  const closeBtn = document.querySelector(".close");

  images.forEach(img => {
    img.addEventListener("click", () => {
      lightbox.style.display = "flex";
      lightboxImg.src = img.src;
    });
  });

  function closeLightbox() {
    lightbox.style.display = "none";
  }

  closeBtn.addEventListener("click", closeLightbox);

  lightbox.addEventListener("click", (e) => {
    if (e.target !== lightboxImg) closeLightbox();
  });

  document.addEventListener("keydown", (e) => {
    if (e.key === "Escape") closeLightbox();
  });
});
</script>
