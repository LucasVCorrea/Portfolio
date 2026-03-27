---
layout: default
title: Berisso
---

<div class="tool-hero">
  <h1>Dashboard de Actividad De Berisso</h1>
  <p class="tool-subtitle">
    Sistema Integral de Recaudación y Análisis para el Municipio de Berisso.
  </p>
  <p>
    Tablero estratégico diseñado para supervisar la actividad recaudatoria, judicial y productiva vinculada a las fotomultas municipales.
  </p>
</div>

---

## Descripción General

<div class="section-block">

El sistema centraliza información clave sobre la gestión de presunciones e infracciones en el Municipio de Berisso, permitiendo el análisis integral de la actividad administrativa, judicial y productiva.

Facilita la toma de decisiones mediante indicadores claros, métricas comparativas y visualizaciones orientadas a la optimización de recursos y procesos.

</div>

---

## Funcionalidades Principales

<div class="feature-grid">

<div class="feature-item">
<h3>Actividad Recaudatoria</h3>
<p>Seguimiento detallado de ingresos generados por fotomultas, evolución temporal y comparación entre períodos.</p>
</div>

<div class="feature-item">
<h3>Actividad Judicial</h3>
<p>Análisis del estado procesal de las infracciones, evolución de causas y métricas de resolución.</p>
</div>

<div class="feature-item">
<h3>Actividad Productiva</h3>
<p>Monitoreo del volumen de actas generadas, procesamiento de infracciones y desempeño operativo.</p>
</div>

<div class="feature-item">
<h3>Gestión de Usuarios</h3>
<p>Control de accesos, perfiles y seguimiento de actividad dentro del sistema.</p>
</div>

</div>

---

## Gestión de Notificaciones

<div class="section-block">

<h3>Lotes de Notificación</h3>
<p>Visualización y seguimiento de los lotes de notificaciones entregadas en la Municipalidad de Berisso.</p>

<h3>Estado y Trazabilidad</h3>
<p>Control del estado de cada lote, fechas de emisión y confirmación de recepción.</p>

<h3>Histórico de Entregas</h3>
<p>Acceso a registros históricos para auditoría y control administrativo.</p>

</div>

---

## Análisis Estratégico

<div class="section-block">

<h3>Métricas Comparativas</h3>
<p>Comparación entre períodos mensuales, trimestrales y anuales para detectar tendencias.</p>

<h3>Indicadores Clave (KPIs)</h3>
<p>Panel de control con métricas fundamentales para la gestión financiera y operativa.</p>

<h3>Visualización Dinámica</h3>
<p>Gráficos interactivos que permiten explorar datos por rango de fechas, tipo de infracción o estado judicial.</p>

</div>
## Vista del Producto

<div class="image-grid">
  <div class="image-card">
    <img src="{{ '/assets/img/Login.png' | relative_url }}" alt="Login">
    <h4>Inicio de Sesión</h4>
  </div>
  <div class="image-card">
    <img src="{{ '/assets/img/Main site.png' | relative_url }}" alt="Dashboard principal">
    <h4>Dashboard Principak</h4>
  </div>
  <div class="image-card">
    <img src="{{ '/assets/img/Actividad por Camaras.png' | relative_url }}" alt="Mapa Interactivo">
    <h4>Mapa Interactivo</h4>
  </div>
  <div class="image-card">
    <img src="{{ '/assets/img/Actividad Juzgados.png' | relative_url }}" alt="Informacion Juzgados">
    <h4>Actividad Judicial</h4>
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
