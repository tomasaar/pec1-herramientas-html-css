# Memoria PEC1 - Herramientas HTML y CSS II

## 1. Introducción
Este documento detalla el proceso de desarrollo de la PEC1 para la asignatura Herramientas HTML y CSS II. El proyecto consiste en un sitio web de una sola página (one-page) de carácter informativo y responsive sobre el paraje natural de las **Lagunas de Ruidera**, aplicando un workflow de desarrollo moderno.

## 2. Proceso de desarrollo
1. **Configuración del entorno**: Clonación del UOC Boilerplate v3.13.0 e instalación de dependencias mediante `npm install`.
2. **Arquitectura de archivos**: Organización del código fuente en la carpeta `src/`, separando la lógica de estilos en `src/scss/` mediante parciales.
3. **Maquetación HTML**: Creación de una estructura semántica para las secciones de Hero, Navegación, Galería, Ubicación (Maps) y Contacto.
4. **Estilado con Sass**: Implementación de un sistema de diseño basado en variables y funciones, utilizando `@use` para la gestión de módulos.
5. **Control de calidad**: Configuración de Stylelint para asegurar la consistencia del código SCSS.
6. **Compilación**: Generación de la versión de producción en la carpeta `dist/` mediante el comando `npm run build`.
7. **Publicación**: Alojamiento del código en GitHub y despliegue continuo en Netlify.

## 3. Decisiones técnicas
- **Arquitectura CSS (BEM)**: Se ha elegido la metodología **BEM (Block Element Modifier)** para garantizar un código escalable y evitar la especificidad excesiva. Ejemplo: `.hero__title`, `.content--gallery`.
- **Estrategia Mobile-First**: El desarrollo se ha realizado pensando primero en dispositivos móviles, utilizando Media Queries para expandir el diseño en pantallas grandes. Esto optimiza el rendimiento y la experiencia de usuario.
- **Sass**:
  - **Variables**: Centralización de colores corporativos y tipografía Montserrat.
  - **Funciones propias**: Se creó `shade()` para generar variaciones de color en estados `:hover` y `responsive-font()` utilizando `clamp()` para una tipografía fluida sin necesidad de múltiples media queries.
  - **Parciales**: División en `_variables.scss`, `_functions.scss`, `_base.scss` y `_layout.scss` para mejorar la mantenibilidad.
- **Dependencias externas**: Se ha integrado **FontAwesome** para la iconografía social y de contacto, y un **iframe de Google Maps** para la sección de ubicación.

## 4. Stylelint
Para asegurar la calidad del código, se ha configurado Stylelint extendiendo las configuraciones estándar de SCSS.
- **Justificación de reglas**:
  - `order/properties-alphabetical-order`: Obliga a un orden claro, facilitando la lectura a otros desarrolladores.
  - `max-nesting-depth: 3`: Evita el "callback hell" de CSS, manteniendo la especificidad baja.
  - `selector-class-pattern`: Asegura que todas las clases sigan el formato kebab-case exigido por BEM.
- **Resultado**: El comando `npm run lint` no devuelve errores, cumpliendo con los estándares de la asignatura.

## 5. Resultados finales
El sitio web es totalmente responsive, adaptándose desde teléfonos móviles hasta pantallas de escritorio de gran formato. La compilación mediante `npm run build` genera un paquete optimizado y minificado en la carpeta `dist/`.

## 6. Enlaces
- GitHub: https://github.com/tomasaar/pec1-herramientas-html-css
- Netlify: https://69c752dc80f14a0008049286--sparkling-basbousa-b77118.netlify.app/
- Video: [PEGA AQUÍ EL ENLACE A TU VÍDEO]

## 7. Evaluación por pares
*Nota: Esta sección se completará tras la revisión de los trabajos de los compañeros asignados.*
- Compañero 1: / 4 puntos. Comentarios: ...
- Compañero 2: / 4 puntos. Comentarios: ...

## 8. Conclusión
Proyecto completado conforme a objetivos y requisitos del enunciado, con especial atención a metodología y buenas prácticas de CSS.
