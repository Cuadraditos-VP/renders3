# Mis renders

Galería para guardar renders ordenados por carpetas. Se instala como app (PWA) y funciona sin conexión.

## Publicar en GitHub Pages

1. Creá un repositorio nuevo en GitHub (por ejemplo `mis-renders`).
2. Subí **todo el contenido de esta carpeta** a la raíz del repositorio: `index.html`, `manifest.webmanifest`, `sw.js`, `.nojekyll` y la carpeta `icons/`.
   - Desde la web: *Add file → Upload files* y arrastrá los archivos y la carpeta.
3. Andá a *Settings → Pages*, en *Source* elegí **Deploy from a branch**, rama `main`, carpeta `/ (root)` y guardá.
4. En uno o dos minutos la app queda en `https://TU-USUARIO.github.io/mis-renders/`.

## Instalarla

- **Android / Chrome / Edge:** botón **Instalar app** de la barra lateral, o menú ⋮ → *Instalar app*.
- **iPhone / iPad (Safari):** botón Compartir → *Agregar a pantalla de inicio*.

## Actualizar

Cuando cambies algo, abrí `sw.js` y subí el número de `VERSION` (`renders-v1` → `renders-v2`). Así los dispositivos que ya la tienen instalada descargan la versión nueva.

## Importante sobre tus imágenes

Los renders se guardan **en el navegador de cada dispositivo** (IndexedDB), no en GitHub. Eso significa que:

- Lo que subas en la compu no aparece en el celular, y viceversa.
- Si borrás los datos del sitio en el navegador, se borran los renders.
- La app pide almacenamiento persistente para que el navegador no los elimine solo por falta de espacio.
