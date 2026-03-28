# Memoria PEC1 - Herramientas HTML y CSS II

## 1. Introducción
Este documento refleja el desarrollo de la PEC1 de la asignatura, basada en un sitio one-page sobre el paraje natural "Lagunas de Ruidera".

## 2. Proceso de desarrollo
1. Clonación/inicialización del proyecto.
2. Creación de estructura de carpetas: `src/`, `src/scss/`, `src/assets/`, `dist/`.
3. Edición de `src/index.html`: secciones principales.
4. Implementación Sass en parciales y `main.scss`.
5. Configuración de Stylelint en `.stylelintrc.json`.
6. Pruebas locales con `npm run stylelint` y `npm run build`.
7. Subida a GitHub y despliegue en Netlify.

## 3. Decisiones técnicas
- **HTML Semántico**: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`.
- **Sass**:
  - Variables: colores, tipografía, medidas.
  - Funciones propias: `shade()` para oscurecer color, `responsive-font()` para adaptabilidad.
  - Anidado BEM.
  - Parciales (`_base`, `_layout`, etc.).
  - `@use` (recomendado en versiones modernas de Sass).
- **Metodología**: BEM + mobile-first.
- **Dependencias externas**: FontAwesome para iconos + iframe de Google Maps.

## 4. Stylelint
- Extiende:
  - `stylelint-config-standard`
  - `stylelint-config-standard-scss`
- Plugins:
  - `stylelint-scss`
  - `stylelint-order`
- Reglas principales:
  - `indentation: 2`
  - `max-nesting-depth: 3`
  - `selector-class-pattern: "^[a-z][a-z0-9-]*$"`
  - `order/properties-alphabetical-order: true`
  - `color-hex-case: lower`
  - `string-quotes: double`
- Resultado: validación sin errores tras ajustes.

## 5. Resultados finales
- Web responsive funcionando.
- `npm run build` genera `dist/` con `css/main.css` + HTML + assets.
- Netlify desplegado correctamente.

## 6. Enlaces
- GitHub: https://github.com/tomasaar/pec1-herramientas-html-css
- Netlify: https://<tu-site>.netlify.app
- Video: https://drive.google.com/drive/folders/<tu-link>

## 7. Evaluación por pares
- Compañero 1: / 4 puntos. Comentarios: ...
- Compañero 2: / 4 puntos. Comentarios: ...

## 8. Conclusión
Proyecto completado conforme a objetivos y requisitos del enunciado, con especial atención a metodología y buenas prácticas de CSS.
