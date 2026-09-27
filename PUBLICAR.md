# Cómo publicar una entrada del blog

No hace falta tocar HTML. Una entrada es **un archivo de texto**.
La lista del blog se actualiza sola.

## 1. Sube las fotos (si las hay)

En GitHub: **Add file → Upload files**, y las sueltas en la carpeta
`images/blog/`. Nombres sin acentos, sin eñes y sin espacios:
`regreso-clases-2026.jpg`.

Los vídeos **no** se suben aquí. Van a YouTube, y en la entrada se pone
el incrustado (ver la plantilla).

## 2. Crea el archivo de la entrada

En GitHub: **Add file → Create new file**.

El nombre tiene que seguir este patrón exacto:

    _posts/AAAA-MM-DD-nombre-corto.md

Por ejemplo: `_posts/2026-10-15-regreso-a-clases.md`

La fecha del nombre es la que ordena el blog. El `nombre-corto` es lo
que saldrá en la dirección: `sponsorachildmexico.org/blog/regreso-a-clases/`

## 3. Copia la plantilla

Está en `_drafts/PLANTILLA.md`. Ábrela, copia todo, pégalo en tu archivo
nuevo y cambia lo que haga falta.

Las líneas entre las dos filas de tres rayas son la ficha de la entrada:

| Línea | Qué es |
|---|---|
| `title` | El título, entre comillas |
| `date` | La fecha, igual que la del nombre del archivo |
| `category` | Una palabra: School, Milestones, The home... |
| `descripcion` | Una frase para Google, unos 150 caracteres |
| `image` | La foto de portada. Quítala si no hay |
| `image_alt` | Qué se ve en la foto, para quien no puede verla |

Debajo de las tres rayas se escribe normal.

## 4. Guarda

Botón verde **Commit changes** → *Commit directly to the main branch*.

En un minuto está publicada. Si no aparece, mira en la pestaña
**Actions** del repositorio: si hay algo en rojo, es que el archivo
tiene una errata (casi siempre la fecha o las comillas del título).

## 5. Cuando el blog deje de ser un borrador

Ahora mismo el blog lleva `noindex`: Google no lo lee, porque las
entradas son de relleno.

Cuando haya entradas de verdad, abre `_config.yml` y cambia:

    blog_borrador: true

por:

    blog_borrador: false

Eso quita el aviso amarillo de la página y deja que Google entre.

---

**Si prefieres no hacer nada de esto**, mándame el texto, las fotos y
el enlace de YouTube y lo publico yo. Esto está aquí para que también
puedas hacerlo tú, sin depender de nadie.
