---
layout: default
title: Automatización de Extracción de Datos
---

<div class="tool-hero">
  <h1>Automatización de Extracción de Datos</h1>
  <p class="tool-subtitle">
    Script de scraping para recopilar información de manera automatizada y generar reportes completos.
  </p>
  <p>
    Herramienta robusta que permite optimizar la recolección de datos, agilizar procesos manuales y centralizar información clave en un archivo CSV.
  </p>
</div>

---

## Descripción General

<div class="section-block">
Este proyecto permite extraer datos de sistemas web de forma automatizada, gestionando inicios de sesión, navegación por secciones, filtrado de información y paginación. 
La información se guarda de manera incremental en un archivo CSV, asegurando que los datos estén siempre actualizados sin duplicaciones.
</div>

---

## Funcionalidades Principales

<div class="feature-grid">

<div class="feature-item">
<h3>Inicio de Sesión Automático</h3>
<p>El sistema inicia sesión de forma segura y controlada, evitando la entrada manual de credenciales.</p>
</div>

<div class="feature-item">
<h3>Navegación Inteligente</h3>
<p>Accede a secciones específicas, aplica filtros y selecciona la cantidad de registros a procesar automáticamente.</p>
</div>

<div class="feature-item">
<h3>Extracción Detallada</h3>
<p>Recopila información organizada de cada registro, incluyendo datos personales, contactos, direcciones y tablas asociadas.</p>
</div>

<div class="feature-item">
<h3>Guardado Incremental</h3>
<p>Los datos se guardan en un CSV de manera incremental, evitando pérdidas o duplicaciones durante la ejecución del script.</p>
</div>

</div>

---

## Flujo de Trabajo

<div class="section-block">
1. Se configura el entorno de automatización con el navegador controlado por el script.  
2. El script inicia sesión en la plataforma web de forma automatizada.  
3. Se navega hasta la sección de interés y se aplican los filtros deseados.  
4. Por cada registro, se accede a detalles adicionales y se extraen los datos relevantes.  
5. Los datos se agregan a un archivo CSV de manera incremental para mantener un registro completo.  
6. Se gestiona automáticamente la paginación hasta que se procesan todos los registros.  
</div>

---

## Vista del Proyecto

<div class="image-grid">
  <div class="image-card">
    <img src="{{ '/assets/img/webscrapcaptura.jpg' | relative_url }}" alt="block code">
    <h4>Bloque de Código</h4>
  </div>
  <div class="image-card">
    <img src="{{ '/assets/img/webscrapresult.jpg' | relative_url }}" alt="result sample">
    <h4>Logs de reportes</h4>
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
