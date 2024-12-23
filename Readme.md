# Animación Hello World con CSS

Este proyecto demuestra una forma creativa de transformar un clásico "Hello World" en una animación visualmente impactante utilizando CSS. La animación incluye:

- Mostrar el texto "HELLO WORLD" con una imagen de fondo recortada al texto.
- Animar el texto para que crezca y gire hasta ocupar toda la pantalla.
- Transición de la imagen al fondo de la página.

## Tabla de Contenidos

- [Animación Hello World con CSS](#animación-hello-world-con-css)
  - [Tabla de Contenidos](#tabla-de-contenidos)
  - [Descripción General](#descripción-general)
  - [Características](#características)
  - [Tecnologías Utilizadas](#tecnologías-utilizadas)
  - [Cómo Funciona](#cómo-funciona)
    - [HTML](#html)
    - [CSS](#css)
      - [Animaciones Principales](#animaciones-principales)
  - [Cómo Ejecutarlo](#cómo-ejecutarlo)
  - [Mejoras Futuras](#mejoras-futuras)

## Descripción General

Este proyecto es una exploración divertida del poder de CSS para crear animaciones y efectos dinámicos en la web. Está diseñado para ser escalable, responsivo y visualmente atractivo en diferentes tamaños de pantalla.

## Características

- **Animación de Texto**: Las letras de "HELLO WORLD" aparecen en pantalla con una imagen de fondo recortada al texto.
- **Escalado y Rotación**: El texto crece y gira hasta que una sola letra ocupa toda la pantalla.
- **Transición de Fondo**: La imagen de fondo se convierte en el fondo de la página de manera fluida.

## Tecnologías Utilizadas

- **HTML5**: Para estructurar el contenido.
- **CSS3**: Para crear animaciones, transiciones y diseños responsivos.

## Cómo Funciona

### HTML

El archivo `index.html` contiene una estructura simple con un contenedor para la animación:

```html
<div class="animation-container">
  <div class="text">HELLO WORLD</div>
</div>
```

### CSS

El archivo `styles.css` incluye estilos y animaciones que dan vida al proyecto.

#### Animaciones Principales

1. **Animación de Entrada**:

   - El texto se desliza desde la derecha y se hace visible.

   ```css
   @keyframes slideIn {
     0% {
       transform: translateX(100%) scale(1);
       opacity: 0;
     }
     50% {
       transform: translateX(0) scale(1);
       opacity: 1;
     }
     100% {
       transform: translateX(0) scale(1);
     }
   }
   ```

2. **Crecimiento y Rotación**:

   - El texto crece y gira hasta ocupar toda la pantalla.

   ```css
   @keyframes growAndRotate {
     0% {
       transform: scale(1) rotate(0deg);
     }
     80% {
       transform: scale(15) rotate(360deg);
     }
     100% {
       transform: scale(15) rotate(360deg);
     }
   }
   ```

3. **Transición del Fondo**:

   - La imagen se convierte en el fondo de la página.

   ```css
   @keyframes fadeInBackground {
     0% {
       opacity: 0;
     }
     100% {
       opacity: 1;
     }
   }
   ```

## Cómo Ejecutarlo

1. Clona este repositorio:

   ```bash
   git clone https://github.com/ManRio/AnimatedHelloWorld
   ```

2. Navega al directorio del proyecto:

   ```bash
   cd animacion-hello-world
   ```

3. Abre `index.html` en tu navegador para ver la animación.

## Mejoras Futuras

- **Personalización**: Añadir controles para personalizar el texto, la imagen o la velocidad de la animación.
- **Accesibilidad**: Incluir roles ARIA y mejorar el soporte para lectores de pantalla.
- **Interactividad**: Permitir a los usuarios reiniciar o pausar la animación.

¡Siéntete libre de bifurcar este proyecto y experimentar! Los PRs son bienvenidos.
