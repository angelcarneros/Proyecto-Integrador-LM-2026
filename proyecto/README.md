# Proyecto Integrador LM 2026 · AnyAnime

**Propietario:** angelcarneros

---

## Palabras del día

- **Meta**
- **Contexto**
- **Día** 

---

## UD3 · Estructura HTML

- Cabecera completa en todas las páginas: `DOCTYPE`, `html lang="es"`, `meta charset` UTF-8, `viewport`, `title` y las meta `description`, `keywords` y `author`.
- Cuerpo organizado en bloques `div` comentados, con un único `h1`, jerarquía de títulos sin saltos y elementos como `hr`, `blockquote`, `pre` y entidades (`&copy;`, `&amp;`, `&#33;`).
- Sitio de varias páginas definido en el mapa del sitio, incluido un catálogo con los datos de `datos.xml`.

---

## Mapa del sitio

| Fichero | title | Qué contiene |
|---|---|---|
| index.html | Inicio \| AnyAnime | Portada: presentación de la web, animes organizados por género, opinión del creador y ficha técnica. |
| catalogo.html | Catálogo \| AnyAnime | Todos los animes de `datos.xml` con su título, género, duración de capítulo y descripción. |
| descripcion-swordartonline.html | Sword Art Online \| AnyAnime | Sinopsis, personajes principales y datos de Sword Art Online. |
| descripcion-jujutsukaisen.html | Jujutsu Kaisen \| AnyAnime | Sinopsis, personajes principales y datos de Jujutsu Kaisen. |
| descripcion-gintama.html | Gintama \| AnyAnime | Sinopsis, personajes principales y datos de Gintama. |
| descripcion-another.html | Another \| AnyAnime | Sinopsis, personajes principales y datos de Another. |
| resenas-swordartonline.html | Reseña de Sword Art Online \| AnyAnime | Reseña y valoración de Sword Art Online. |
| resenas-jujutsukaisen.html | Reseña de Jujutsu Kaisen \| AnyAnime | Reseña y valoración de Jujutsu Kaisen. |
| resenas-gintama.html | Reseña de Gintama \| AnyAnime | Reseña y valoración de Gintama. |
| resenas-another.html | Reseña de Another \| AnyAnime | Reseña y valoración de Another. |

--- 

### Errores del validador W3C

| Página | Errores encontrados | Cómo lo corregí |
|---|---|---|
| index.html | 0 errores | No hizo falta corregir nada. |
| catalogo.html | 0 errores | No hizo falta corregir nada. |
| descripcion-swordartonline.html | 0 errores | No hizo falta corregir nada. |
| descripcion-jujutsukaisen.html | 0 errores | No hizo falta corregir nada. |
| descripcion-gintama.html | 0 errores | No hizo falta corregir nada. |
| descripcion-another.html | 0 errores | No hizo falta corregir nada. |
| resenas-swordartonline.html | 0 errores | No hizo falta corregir nada. |
| resenas-jujutsukaisen.html | 0 errores | No hizo falta corregir nada. |
| resenas-gintama.html | 0 errores | No hizo falta corregir nada. |
| resenas-another.html | 0 errores | No hizo falta corregir nada. |
| datos.xml | "Schema Error": el validador W3C es de HTML y el XML no declara esquema. | No es un error del fichero: comprobé que está bien formado abriéndolo en el navegador. |

---

## UD5 · Tablas y formularios
- Añadida tabla de personajes principales de los animes de AnyAnime

---

## UD6 · HTML5 semántico, formularios y multimedia

### Reto 1 · Estructura semántica

- `index.html` y `descripcion-swordartonline.html` pasan a la estructura de HTML5: `header` con logo y `nav`, un único `main`, `section`, `article`, `aside` y `footer`.
- Eliminados los `div` que solo servían para maquetar en esas páginas.
- `meta author` con mi usuario y firma `<p id="firma-angelcarneros">` en el `footer` de todas las páginas.

### Reto 2 · Formulario HTML5

- Formulario de `contacto.html` con 6 tipos de input de HTML5: `email`, `url`, `tel`, `date`, `number` y `range`, además de `select`, `checkbox`, `radio` y `textarea`.
- Atributos de validación: `required`, `placeholder`, `min`/`max`/`step`, `minlength`/`maxlength` y un `pattern` para el teléfono (9 dígitos empezando por 6, 7, 8 o 9) con su `title` explicativo.
- Cada campo con su `<label for="…">`.
- Sección "Notas de nuestras reseñas" con un `meter` por anime para mostrar su valoración sobre 10.

### Reto 3 · Multimedia e interactivos

- `audio` con `controls` y dos `source` (OGG y MP3) guardados en `media/`, con texto alternativo y enlace de descarga.
- Tráileres oficiales de YouTube insertados con `iframe` en cada género de la portada.
- Portadas de los animes en `figure` con su `figcaption` (anime, estudio y año).
- Sección de preguntas frecuentes con 4 `details`/`summary`, la primera abierta con `open` y una respuesta que muestra etiquetas escritas con `&lt;` y `&gt;`.
