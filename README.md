# NexoPlay - Plataforma de Streaming de eSports

## Portada
- **Integrante:** [Adriana Imelda Cnales Pérez]
- **Módulo:** Módulo 2- introducción a CSS moderno, git y github 
- **Fecha:** 27 de junio de 2026

## Auditoría de Diseño
Para este rediseño, se utilizó **CSS Grid** para la arquitectura global (Macro-Layout) permitiendo una disposición de dos columnas (menú y contenido principal), y **Flexbox** para las tarjetas de contenido (Micro-Layout), asegurando una alineación vertical perfecta de los elementos multimedia.

## Reto IA (Optimización de Estilos)
* **Prompt enviado:** "Actúa como Ingeniero Frontend Senior. Optimiza el siguiente bloque de código CSS (el estilo de la clase .card). Asegúrate de implementar variables CSS, garantizar un contraste de color AAA según WCAG y usar Flexbox para el centrado vertical. Devuélveme solo el código CSS optimizado."
* **CSS Original:** /* CSS Original (sin estructura) */
.card {
    border: 1px solid black;
    width: 200px;
    padding: 10px;
}
.card img {
    width: 100%;
}
* **CSS Optimizado por la IA:** /* CSS Optimizado con Flexbox y variables */
.card {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 1rem;
    border: 1px solid var(--color-borde);
    border-radius: 8px;
    background: #1e1e1e;
}

## Análisis Crítico
1. **¿El código generado por la IA respetó el diseño responsivo?** Sí, al combinarlo con nuestras consultas de medios (`@media`), el código se integra perfectamente.
2. **¿Qué ventajas técnicas aportó la refactorización?** La IA permitió el uso de variables CSS (`:root`), lo que mejora la mantenibilidad del código, y aseguró que el espaciado interno (padding/margin) fuera más eficiente para cumplir con los estándares de accesibilidad AAA.

## Accesibilidad y SEO
Se han utilizado etiquetas semánticas (`<header>`, `<nav>`, `<main>`, `<article>`) y atributos `alt` descriptivos en las imágenes. Esto es fundamental para que los lectores de pantalla puedan interpretar el contenido, mejorando el posicionamiento SEO y la inclusión digital.