# Ay Bendito Chiringuito — web

Web de una sola página + página de carta. Todo es HTML estático: se sube tal cual
a Vercel, Netlify o cualquier alojamiento.

## Archivos
- `index.html` … página principal (portada, la casa, espetos, carta resumida, música, galería, contacto)
- `carta.html` … carta completa con todos los platos y precios
- `img/` … logos y fotos

## Lo que conviene cambiar (todo marcado en el código)
- **Teléfono / WhatsApp**: busca `600000000` y `34600000000` en los dos .html y pon el número real.
  (WhatsApp lleva el 34 delante y sin espacios: `34952XXXXXX`.)
- **Dirección**: en `index.html` busca `DIRECCIÓN`.
- **Horario**: en `index.html` busca `HORARIO`.
- **Carta y precios**: todo está en `carta.html`. Cada plato es una línea como:
  `<li><span class="d">Gambas</span><span class="dots"></span><span class="pr">16,50 €</span></li>`
  Cambia el nombre o el precio sin tocar las etiquetas `< >`.

## Cómo cambiar una foto
Sustituye el archivo dentro de `img/` por otro con el MISMO nombre
(por ejemplo, una nueva `portada.jpg`), o cambia la ruta en el HTML.

## Subir a Vercel con GitHub (recomendado)
1. Crea un repositorio en github.com y sube esta carpeta (botón "Add file → Upload files").
2. En vercel.com: "Add New → Project", elige el repositorio y "Deploy".
3. Para editar después: entra al archivo en github.com, pulsa el lápiz ✏️, edita,
   "Commit changes" y Vercel publica solo en unos segundos.
