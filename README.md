# NUDAS — Cafetería Online & Café de Especialidad

> **"Un café que desata momentos."**  
> Experiencia web inmersiva para **NUDAS** (`@nudas_co`), marca chilena de café de especialidad tostado en grano (250 g) y filtros portátiles por goteo individual (**SipO's**, 105 g).

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/shdwwrr/nudas-cafe)
[![GitHub Pages](https://img.shields.io/badge/Live-GitHub%20Pages-2ea44f?style=flat&logo=github)](https://shdwwrr.github.io/nudas-cafe/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

---

## 🌐 Enlaces en Vivo

- **Producción (GitHub Pages):** [https://shdwwrr.github.io/nudas-cafe/](https://shdwwrr.github.io/nudas-cafe/)
- **Despliegue en Render:** [Desplegar en Render con 1 Clic](https://render.com/deploy?repo=https://github.com/shdwwrr/nudas-cafe)
- **Repositorio Oficial:** [https://github.com/shdwwrr/nudas-cafe](https://github.com/shdwwrr/nudas-cafe)

---

## ✨ Características Principales

1. **Hero Cinemático Sin Cortes Duros:**
   - Video loop fluido de 7 segundos en H.264 (`nudas-hero-loop.mp4`) optimizado con iluminación volumétrica y partículas suspendidas.
   - Capa orgánica de gradiente `.hero-edge` que fusiona el hero con el fondo sin bordes marcados.
   - Pila tipográfica con *Instrument Sans* y *Newsreader Italic*.

2. **Escultura 3D Interactiva con Three.js:**
   - Nudo en forma de ocho en 3D interactivo que responde al movimiento del cursor o toque móvil.
   - Granos de café 3D orbitando suavemente alrededor del nudo central.
   - Sistema de partículas flotantes con renderizado de atmósfera cálida a 60 FPS.

3. **Catálogo Oficial NUDAS (Precios y Orígenes Lider.cl):**
   - **Café en Grano (250 g) — $10.990 CLP:**
     - Colombia Huila (Tostado Medio)
     - Costa Rica Tarrazú
     - Guatemala Antigua
     - Honduras Marcala
     - El Salvador Apaneca
     - Bolivia Yungas Caranavi
   - **SipO's Drip Bags (105 g / 10 sobres) — $7.590 CLP:**
     - Filtros individuales de goteo listos para infusionar en taza en cualquier lugar.
   - Filtro interactivo por formato (*Todos*, *Café en Grano*, *SipO's Drip Bags*).
   - Acceso directo para compra en canales oficiales (Lider.cl / SumUp).

4. **Experiencia Responsiva & Accesible:**
   - Arquitectura CSS fluida con `clamp()` para tipografías y espaciados dinámicos.
   - Soporte completo para `prefers-reduced-motion` (pausa de animaciones intensivas y fallback a póster de alta definición).
   - 100% libre de dependencias pesadas: carga instantánea en cualquier conexión.

---

## 🚀 Despliegue en Render

El proyecto incluye configuración nativa de infraestructura como código en [`render.yaml`](./render.yaml).

### Opción A: Despliegue Automático con 1 Clic
Haz clic en el botón:  
[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/shdwwrr/nudas-cafe)

### Opción B: Blueprint en Render Dashboard
1. Ingresa a [dashboard.render.com](https://dashboard.render.com/).
2. Haz clic en **New +** > **Blueprint**.
3. Selecciona el repositorio `shdwwrr/nudas-cafe`.
4. Render leerá automáticamente el archivo `render.yaml` y desplegará el sitio estático con soporte HTTPS global y CDN.

---

## 💻 Ejecución Local

No requiere compilación previa. Puedes ejecutarlo con cualquier servidor local:

```bash
# Con Node.js integrado
node server.js

# O con npx serve
npx serve . -l 3000

# O con Python
python -m http.server 3000
```

Abre tu navegador en `http://localhost:3000`.

---

## 📁 Estructura del Proyecto

```
nudas-cafe/
├── .github/
│   └── workflows/
│       └── deploy.yml        # CI/CD automático para GitHub Pages
├── media/
│   ├── lider/                # Empaques oficiales NUDAS recortados en alta definición
│   │   ├── grano-*.png
│   │   └── sipo-*.png
│   ├── nudas-hero-loop.mp4   # Loop cinemático de fondo (7s H.264)
│   ├── nudas-hero-bg-clean.jpg
│   └── nudas-logo-light.png  # Isotipo y logotipo oficial NUDAS
├── index.html                # Código fuente principal (HTML5, Three.js, CSS3)
├── package.json              # Metadatos del proyecto y scripts
├── render.yaml               # Manifiesto Blueprint de Render
├── server.js                 # Servidor HTTP estático nativo Node.js
└── README.md
```

---

## ☕ Créditos
- Marca: **NUDAS Cafetería Online** ([@nudas_co](https://www.instagram.com/nudas_co/))
- Desarrollado con Three.js, Canvas WebGL y Modern Web Standards.
