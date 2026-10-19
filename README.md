# Portafolio

Sitio estático de una sola página. No necesita build: todo lo que se publica está en `public/`.

```
public/
  index.html   página principal
  404.html     página para links que no existen
  _headers     cabeceras de seguridad
  robots.txt
wrangler.toml  configuración de Cloudflare Pages
```

## Publicar en Cloudflare Pages

El sitio está conectado a Cloudflare Pages y se publica solo con cada push a `main`. `wrangler.toml` le indica a Pages que publique la carpeta `public/`, así que no hace falta configurar comando de build ni directorio de salida en el panel.

Para verla localmente antes de subirla: `npx wrangler pages dev` y abrí http://localhost:8788.

## Antes de publicar

Completá los textos entre corchetes en `public/index.html` (nombre, mes, proyectos, links de demo, WhatsApp, email y redes).
