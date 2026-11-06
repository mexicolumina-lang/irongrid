# IRONGRID (PWA)

App de gym que corre entera en el teléfono: funciona sin señal y se instala en Android y iPhone. Los datos se guardan en el teléfono y, si quieres, se respaldan en un repo privado de GitHub.

## 1. Publicarla (GitHub Pages, gratis)

1. Crea un repo **público** (por ejemplo `irongrid`) y sube estos archivos: `index.html`, `sw.js`, `manifest.webmanifest`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`. Es solo el código, sin datos.
2. En el repo: Settings > Pages > Source: *Deploy from a branch* > rama `main`, carpeta `/ (root)`.
3. En un minuto tendrás un link tipo `https://tu-usuario.github.io/irongrid/`.

## 2. Instalarla

- **iPhone**: abre el link en **Safari** > Compartir > *Añadir a pantalla de inicio*.
- **Android**: abre el link en Chrome > menú ⋮ > *Instalar app*.

Ábrela una vez con señal para que se guarde offline. Después funciona sin conexión.

## 3. Respaldo en GitHub (recomendado)

Usa un **repo privado distinto** al de la app, solo para datos. Crea un token fine-grained con acceso solo a ese repo y permiso **Contents: Read and write**. En Ajustes de la app rellena repo (`usuario/repo-datos`), rama, archivo y token, y pulsa *Subir ahora*. Después sube solo, unos segundos tras guardar, cuando hay señal. El token queda guardado en ese teléfono: configúralo una vez por dispositivo.

Para traer tus datos de la versión Streamlit, pon como archivo `data/users/<tu-perfil>.json` y pulsa *Descargar*. El formato es el mismo.

## Notas

- Cada persona usa su propio teléfono con sus propios datos; no hay perfiles en esta versión.
- Si se reemplaza el código, sube `sw.js` con otro número en `irongrid-v1` para forzar la actualización.
- Un APK se puede generar desde el link publicado con [PWABuilder](https://www.pwabuilder.com). En iPhone solo existe la instalación desde Safari.
