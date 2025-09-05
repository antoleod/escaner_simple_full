# Escáner Web Pro (PWA)

PWA simple para escanear códigos con la cámara (ZXing), guardar resultados en `localStorage`, y exportar a CSV.
Funciona en HTTPS o `localhost`.

## Estructura
```
.
├─ index.html
├─ sw.js
├─ manifest.webmanifest
├─ icons/
│  ├─ icon-192.png
│  └─ icon-512.png
└─ .github/workflows/pages.yml
```

## Cómo publicar en GitHub Pages
1. Crea un repositorio nuevo y sube estos archivos (rama `main`).
2. Ve a **Settings → Pages** y en **Build and deployment** elige **Source: GitHub Actions**.
3. La acción **Deploy static content to Pages** se ejecutará y publicará tu sitio en HTTPS.
4. Abre la URL de Pages (necesaria para que la cámara funcione).

> Si prefieres sin Actions, desactiva el workflow y en **Settings → Pages** elige **Source: main / root**.

## Notas de cámara
- Usa HTTPS o `http://localhost` (no funciona desde `file:///`).
- Da permiso de **Cámara** al sitio.
- En iOS/Safari, el flash/zoom puede no estar disponible en algunos modelos.
