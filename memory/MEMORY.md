# Portfolio — Marc Morlá Isern

## Stack
- Astro + SCSS (BEM) — sin framework JS
- Fuente: Montserrat (Google Fonts)

## Estructura de archivos clave
- `src/layouts/layout.astro` — layout global con meta tags
- `src/pages/` — index, about, proyects, contact
- `src/components/` — header, footer, hero, grid, form, about
- `src/styles/` — organizado en base/, components/, mixins/, sections/, variables/

## Convenciones
- BEM estricto: `.s-` para secciones, `.c-` para componentes
- Variables CSS en `_variables.scss` (grises: --gray-50 a --gray-800, sin --gray-400)
- Mixin `container()` en `_container.scss` para max-width centrado
- Mixin `breakpoint()` en `_breakpoint.scss` (tablet-small: 30rem, tablet: 48rem, desktop: 64rem)
- Dark mode con `prefers-color-scheme: dark` en `:root` de cada archivo SCSS
- Cada sección tiene su propio `_s-nombre.scss` importado en `sections/_index.scss`

## Rutas del header/footer
- Prefijo `/portfolio/` en todos los hrefs (GitHub Pages)

## Estado del proyecto
- Formulario: Formspree integrado (`xpqyzzvg`) en `form.astro`
- Grid de proyectos: datos en array dentro de `grid.astro`, prop `limit` para home (limit=4)
- Logos: pendientes de asset (src="" en header y footer)
- GitHub footer: `https://github.com/maaarcmorla`
- Páginas about y proyects: base completada con contenido genérico
