---
title: 🎨 Aplicación de Matrículas para Escuela de Bellas Artes
publishDate: 2020-03-02 00:00:00
img: /assets/works/aplicacion-control-matricula.webp
img_hover: /assets/works/aplicacion-control-matricula-hover.webp
img_alt: Interfaz moderna para una aplicación académica enfocada en artes
description: |
  Aplicación web desarrollada con React y APIs en Go para gestionar matrículas, estudiantes y transacciones en una escuela de bellas artes.
tags:
  - Desarrollador
  - Diseñador
  - React
---

### 🎨 Aplicación de Matrículas para Escuela de Bellas Artes

**Una solución digital para organizar el arte.**

Esta aplicación web fue creada para una escuela de bellas artes que ofrece cursos de danza, pintura, música y más. Su objetivo es facilitar la gestión de estudiantes, tutores, matrículas y transacciones de una forma ordenada, moderna y accesible. El frontend fue desarrollado con **React**, mientras que el backend, encargado de las APIs REST, fue construido en **Go**.

> 💬 *"El arte inspira, pero también se administra. Esta herramienta conecta ambos mundos con estilo."*

---

### 🛠️ Funcionalidades principales

La aplicación abarca todas las necesidades administrativas de una institución artística:

- 👩‍🎨 **Registro de estudiantes y tutores**  
  Ingreso ágil de información personal.

- 🖌️ **Gestión de cursos artísticos y matrículas**  
  Asignación de estudiantes a cursos como danza, pintura o música, con historial completo.

- 🔐 **Control de acceso por roles**  
  Tres niveles de acceso: **Administrador**, **Operador** y **Visualizador**, según responsabilidades.

- 💳 **Registro y control de transacciones**  
  Gestión de pagos, historial y gráficos básicos.

- 📊 **Dashboard visual e intuitivo**  
  Panel con métricas clave y navegación organizada por secciones.

---

### ⚙️ Tecnologías utilizadas

- 💻 **Frontend**: React.js, Tailwind, TypeScript  
- 🔌 **Backend/API**: Go (Golang)  
- 📱 **Responsive Design**: Funciona perfectamente en móviles

---

### 🖼️ Galería de imágenes

Una muestra visual de las secciones y diseño de la aplicación de control de matrículas:

<!-- Galería -->
<div style="display: flex; flex-wrap: wrap; gap: 20px; justify-content: center; margin-top: 30px;">
  <img src="/assets/works/aplicacion-control-matricula-hover.webp" alt="Pantalla principal"
    onclick="openModal(this.src)" class="galeria-img">
  <img src="/assets/works/aplicacion-control-matricula-2.webp" alt="Registro estudiantes"
    onclick="openModal(this.src)" class="galeria-img">
  <img src="/assets/works/aplicacion-control-matricula-5.webp" alt="Perfil tutor"
    onclick="openModal(this.src)" class="galeria-img">
  <img src="/assets/works/aplicacion-control-matricula-3.webp" alt="Gestión cursos"
    onclick="openModal(this.src)" class="galeria-img">
  <img src="/assets/works/aplicacion-control-matricula-4.webp" alt="Perfil tutor 2"
    onclick="openModal(this.src)" class="galeria-img">
  <img src="/assets/works/aplicacion-control-matricula-6.webp" alt="Perfil tutor 3"
    onclick="openModal(this.src)" class="galeria-img">
</div>

<!-- Modal oculto -->
<div id="imageModal" style="margin: 0; display: none; position: fixed; z-index: 9999; top: 0; left: 0; width: 100%; height: 100%; background-color: rgba(0,0,0,0.8); justify-content: center; align-items: center;">
  <span onclick="closeModal()" style="position: absolute; top: 20px; right: 10px; font-size: 40px; color: white; cursor: pointer;">&times;</span>
  <img id="modalImage" style="max-width: 90%; max-height: 90%; border-radius: 12px; box-shadow: 0 0 25px rgba(255,255,255,0.3); transform: scale(1.05);">
</div>


---



> 🌟 *Una herramienta que da ritmo y orden a la educación artística.*


<style>
  .galeria-img {
    width: 300px;
    border-radius: 12px;
    cursor: pointer;
    transition: box-shadow 0.3s ease-in-out, transform 0.3s ease-in-out;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  }

  .galeria-img:hover {
    box-shadow: 0 200px 400px rgba(0, 0, 0, 0.4);
    transform: translateY(-4px);
  }
</style>



<!-- JS para modal -->
<script>
  function openModal(src) {
    document.getElementById("modalImage").src = src;
    document.getElementById("imageModal").style.display = "flex";
  }

  function closeModal() {
    document.getElementById("imageModal").style.display = "none";
  }

  // Cerrar al hacer clic fuera de la imagen
  document.getElementById("imageModal").addEventListener("click", function (e) {
    if (e.target.id === "imageModal") {
      closeModal();
    }
  });

  document.addEventListener("keydown", function (e) {
    if (e.key === "Escape") {
      closeModal();
    }
  });
</script>