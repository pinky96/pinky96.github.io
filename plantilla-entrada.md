---
# =============================================================
# PLANTILLA PARA UNA ENTRADA NUEVA DEL BLOG — copia este archivo.
#
# Cómo publicar una entrada, paso a paso:
#
# 1. Copia este archivo dentro de la carpeta _posts/ con el nombre:
#       AAAA-MM-DD-titulo-corto-sin-tildes.md
#    Ejemplo: 2026-11-15-vigilancia-y-territorio.md
#    (la fecha del nombre es la fecha de publicación, y el
#    "titulo-corto" se vuelve la URL: /blog/titulo-corto/)
#
# 2. Sube la imagen de la entrada a assets/images/posts/
#    (ideal: formato horizontal, unos 1200x630 píxeles)
#
# 3. Rellena los campos de abajo y escribe el texto al final.
#
# 4. Guarda, haz commit y push. GitHub Pages publica solo.
#
# Este archivo NO se publica: está en la lista "exclude"
# de _config.yml.
# =============================================================

# El layout "post" es la plantilla de entrada (no cambiar).
layout: post

# Título de la entrada, entre comillas.
title: "Aquí va el título de la entrada"

# Fecha de publicación (debe coincidir con la del nombre del archivo).
date: 2026-01-01

# Una o más categorías, entre corchetes y separadas por comas.
# Ejemplos: [seguridad digital], [comunidad, territorio]
categorias: [general]

# Resumen de una o dos frases: aparece en la tarjeta de la portada
# y cuando se comparte el enlace en redes.
resumen: "Un resumen corto de la entrada, de una o dos frases."

# Ruta de la imagen destacada (la que subiste en el paso 2).
imagen: /assets/images/posts/nombre-de-la-imagen.jpg

# Descripción de la imagen para lectores de pantalla (accesibilidad).
imagen_alt: "Qué se ve en la imagen, descrito en una frase"

# Crédito de la imagen (opcional: borra esta línea si no aplica).
imagen_credito: "Foto: nombre de quien la tomó o fuente"
---

Aquí empieza el texto de la entrada, escrito en Markdown.

Puedes usar **negritas**, *cursivas*, [enlaces](https://ejemplo.org) y:

## Subtítulos como este

- listas
- de puntos

> Citas destacadas como esta.

Y más imágenes dentro del texto:

![Descripción de la imagen](/assets/images/posts/otra-imagen.jpg)
