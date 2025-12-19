# Demo estática lista para Cloudflare Pages

Este repositorio está preparado para subir una web estática (HTML/CSS/JS) al plan gratuito de Cloudflare Pages. Solo tienes que sustituir los archivos de ejemplo por los definitivos y conectar el repo en Cloudflare.

## 📂 Estructura
```
public/
├── index.html         # Página de ejemplo (reemplázala por la tuya)
├── styles/            # CSS
├── js/                # JavaScript
├── images/            # Imágenes (vacía, con .gitkeep)
└── fonts/             # Fuentes (vacía, con .gitkeep)
```

> Los archivos de tu captura (HTML, CSS, JS, imágenes y fuentes) pueden colocarse directamente dentro de `public/` respetando sus carpetas.

## 🚀 Despliegue en Cloudflare Pages (plan gratuito)
1. Crea un proyecto nuevo en Cloudflare Pages y selecciona este repositorio.
2. **Framework preset:** `None` / `Static`.
3. **Build command:** déjalo vacío (no es necesario compilar).
4. **Output directory:** `public`.
5. Publica. Cada push generará una preview y, si lo activas, despliegue automático a producción.

## 🔄 Flujo recomendado
- Trabaja en ramas `feature/*` y abre Pull Requests hacia `staging` o `main`.
- Incluye en los PR una nota rápida del cambio y la URL de la preview de Pages.
- Antes de desplegar a producción, revisa enlaces principales y que no haya secretos en el código.

## 🧪 Qué incluye la demo
- Maquetado mínimo en `public/index.html` con indicaciones de estructura.
- Estilos base en `public/styles/main.css`.
- Script mínimo en `public/js/main.js` para verificar carga de JS.

Sustituye o elimina estos archivos cuando pegues el proyecto real. No necesitas pasos adicionales para que Cloudflare Pages lo sirva.
