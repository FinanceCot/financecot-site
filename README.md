# FinanceCot — GitHub Pages (Jekyll)

Repo listo para publicar en **GitHub Pages** con posts en **Markdown**.

## Publicación
1. Crea un repositorio (público) en GitHub, por ejemplo `financecot`.
2. Sube **todos los archivos** de esta carpeta (no subas el ZIP).
3. Ve a **Settings → Pages** y elige **Deploy from a branch** con `main` y carpeta raíz `/`.
4. (Dominio) Mantén el archivo **CNAME** con `www.financecot.com` y en tu registrador crea CNAME `www` → `TU-USUARIO.github.io`. Redirige la raíz `financecot.com` a `https://www.financecot.com` (301).

## Añadir artículos
- Crea un archivo en `/_posts/` con formato `YYYY-MM-DD-mi-titulo.md`.
- Cabecera mínima:
  ```yaml
  ---
  layout: post
  title: "Mi título SEO"
  date: 2025-08-14
  reading_time: 6
  ---
  ```
- Escribe en Markdown. El **disclaimer** se inserta automáticamente desde `_includes/disclaimer.html`.

## Editar navegación/páginas
- Menú en `_includes/header.html`.
- Footer en `_includes/footer.html`.
- Páginas: `sobre.md`, `recursos.md`, etc.

## SEO
- `robots.txt` y `sitemap.xml` incluidos (básico). Puedes activar `jekyll-sitemap` en `_config.yml` si quieres sitemap automático.

## Estilos
- **Tailwind vía CDN** (sin build). Si deseas Tailwind "real", puedes migrar a Astro/Eleventy más adelante.
