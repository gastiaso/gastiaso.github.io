# gastiaso.github.io

Web personal de Guillermo Astiaso: portada con los proyectos y, más adelante, artículos.

Es el sitio de usuario de GitHub Pages: se sirve en la raíz (`https://gastiaso.github.io/`) y los sitios de proyecto (`/barometros/`, `/historias/`, `/de-renta-en-renta/`, `/porra-electoral/`) cuelgan de él. Si se configura un dominio propio en este repositorio, los sitios de proyecto lo heredan.

## Ficheros

| Fichero | Contenido |
|---|---|
| `index.html` | Portada: presentación, proyectos y contacto. HTML y CSS en un solo fichero, sin dependencias externas |
| `sitemap.xml` | Portadas de los proyectos, para enviar en Search Console |
| `.nojekyll` | Publica los ficheros tal cual, sin pasar por Jekyll |

## Publicación

Settings › Pages › Build and deployment › Source: **Deploy from a branch**, rama `main`, carpeta `/ (root)`. Cada push a `main` publica.

## Al activar el dominio propio

1. Verificar el dominio en los ajustes del perfil de GitHub (registro TXT).
2. Settings › Pages › Custom domain en este repositorio; registros DNS A, AAAA y CNAME de `www`; *Enforce HTTPS*.
3. Sustituir `https://gastiaso.github.io` por el dominio nuevo en `index.html` (canonical, og:url, JSON-LD, enlaces e imágenes) y en `sitemap.xml`.
4. Hacer lo mismo en los demás repositorios (canonical, og:url, hreflang, sitemaps, `CITATION.cff`, README).
5. Search Console: propiedad de dominio verificada por DNS; enviar `sitemap.xml` y los sitemaps de cada proyecto.
