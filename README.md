🧩 Proyecto Final — Migración a React (Resumen)

Este proyecto consiste en la migración completa de un sitio previamente desarrollado en HTML y CSS, transformándolo en una aplicación modular con React, utilizando Vite como entorno de desarrollo y React Router DOM para la navegación.

La estructura del proyecto se reorganizó siguiendo buenas prácticas:

components/: Navbar, Hero, ServicesSection, ServiceCard, PortfolioSection, PortfolioRow, AboutSection, ContactSection, Footer.

pages/: Home y ContactPage.

styles/: CSS modularizado por componente.

utils/: funciones auxiliares como ScrollToHashElement.

Uso de assets desde src/assets.

✔ Componentización

Cada sección del sitio fue convertida en un componente independiente.
El Hero, los servicios y el portfolio reciben contenido mediante props.
El formulario de contacto fue migrado a un componente controlado, utilizando useState y manejando eventos con event.preventDefault().

✔ Interactividad

Formulario controlado (useState en cada input).

Submit y reset funcionando.

Datos mostrados por consola.

✔ Navegación

El proyecto usa React Router v6, con dos rutas principales:

/ → Home

/contacto → ContactPage

También se implementó navegación por hash (#servicios, #portfolio, #nosotros) con un componente especial que realiza scroll suave.

✔ Animaciones

Se incorporó Framer Motion para agregar transiciones entre páginas con efectos de fade-in y fade-out.

✔ Estilos

Se mantuvo el diseño original, incluyendo tipografías, botones animados, banner dinámico, layout y estilos responsive.
Cada componente tiene su propio archivo CSS para mantener la organización.

✔ Deploy

El sitio se publicó usando GitHub Pages, ajustando el base en vite.config.js y moviendo la carpeta dist a docs.
