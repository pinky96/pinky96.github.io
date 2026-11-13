# Señales del Micelio

Bitácora personal de imágenes y escritos — tecnología, sociedad civil
y otras señales — publicada en **https://pinky96.github.io** con
[Jekyll](https://jekyllrb.com/) y GitHub Pages.

## Cómo publicar una entrada

1. Copia `plantilla-entrada.md` dentro de `_posts/` con el nombre
   `AAAA-MM-DD-titulo-corto.md` (ejemplo:
   `2026-11-15-vigilancia-y-territorio.md`).
2. Sube la imagen de la entrada a `assets/images/posts/`
   (ideal: horizontal, unos 1200×630 píxeles).
3. Rellena los campos de la cabecera (título, fecha, resumen, imagen)
   y escribe el texto en Markdown. La propia plantilla explica cada campo.
4. Haz commit y push a la rama principal: GitHub Pages reconstruye y
   publica el sitio solo (tarda 1 o 2 minutos).

## Estructura del repositorio

```
_config.yml          Configuración general (título, URL, portada…)
_posts/              Las entradas del blog, una por archivo
_layouts/            Plantillas de página
  default.html         esqueleto común (head + cabecera + pie)
  home.html            portada: columna única con las entradas
  post.html            una entrada individual
  page.html            páginas sueltas (Sobre, 404)
_includes/           Piezas reutilizables
  head.html            metadatos, fuentes, hoja de estilos
  header.html          cabecera con el título glitch y el menú
  footer.html          pie de página
  fecha.html           fechas en español ("29 de mayo de 2026")
  micelio.html         divisor SVG con hilos de micelio
assets/
  css/style.scss       todos los estilos (las variables de color y
                       tipografía están al inicio, comentadas)
  images/posts/        imágenes de las entradas
index.md             La portada (usa el layout "home")
sobre.md             Página "Sobre el proyecto" (/sobre/)
404.html             Página de error
plantilla-entrada.md Plantilla comentada para entradas nuevas
```

## Cómo cambiar la apariencia

- **Colores y tipografías**: todo está en variables al inicio de
  `assets/css/style.scss`, con comentarios que explican cada una.
- **Título, lema, cantidad de entradas en portada**: en `_config.yml`.
- **Menú de navegación**: en `_includes/header.html`.

## Probar el sitio en tu computadora (opcional)

Necesitas Ruby instalado. Luego:

```bash
bundle install            # solo la primera vez
bundle exec jekyll serve  # abre http://localhost:4000
```

No es obligatorio: también puedes editar directo en GitHub y dejar
que GitHub Pages construya el sitio al hacer push.

## Ideas para más adelante

- Paginación cuando haya muchas entradas (plugin `jekyll-paginate`).
- Página de archivo por categorías.
- Buscador sencillo con JavaScript.
