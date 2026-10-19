# Portafolio

Sitio estático de una sola página. No necesita build: todo lo que se publica está en `public/`.

```
public/
  index.html   página principal
  404.html     página para links que no existen
  _headers     cabeceras de seguridad
  robots.txt
wrangler.jsonc configuración de Cloudflare
```

## Publicar en Cloudflare

**Opción A, desde el panel (recomendada):** en Cloudflare, Workers & Pages › Create › Import a repository, elegí este repo y la rama. Cloudflare lee `wrangler.jsonc` y publica `public/`. Si te pide comando de build, dejalo vacío; el de deploy es `npx wrangler deploy`. Cada push a la rama vuelve a publicar.

**Opción B, desde la terminal:**

```sh
npx wrangler login
npx wrangler deploy
```

Para verla localmente antes de subirla: `npx wrangler dev` y abrí http://localhost:8787.

## Antes de publicar

Completá los textos entre corchetes en `public/index.html` (nombre, mes, proyectos, links de demo, WhatsApp, email y redes).
