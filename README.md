# RUSH & GUN

Versión web adaptable e instalable del juego 2D original.

## Publicar en GitHub Pages
1. Creá un repositorio en GitHub.
2. Subí **todo el contenido** de esta carpeta (no solamente el ZIP).
3. Entrá en **Settings → Pages**.
4. En **Build and deployment**, elegí **Deploy from a branch**.
5. Seleccioná `main` y `/ (root)`, y guardá.
6. Esperá a que GitHub Pages publique el sitio. Compartí la URL `https://TU-USUARIO.github.io/TU-REPOSITORIO/`.

## Archivos
- `index.html`: juego, portada de inicio y controles táctiles.
- `manifest.webmanifest`: configuración instalable PWA.
- `sw.js`: caché para permitir abrir el juego luego de la primera carga.
- `assets/portada.jpg`: portada enviada.
- `assets/icon-192.png` y `assets/icon-512.png`: íconos de instalación.
- `assets/whatsapp-preview.jpg`: imagen horizontal para compartir.

## Instalación en el teléfono
- **Android (Chrome):** abrí la URL publicada y elegí “Instalar aplicación” o “Agregar a pantalla de inicio”.
- **iPhone (Safari):** abrí la URL, tocá Compartir y luego “Agregar a pantalla de inicio”.

## Vista previa de WhatsApp
Los metadatos Open Graph están configurados en `index.html`. Para que WhatsApp muestre la miniatura, el juego debe estar publicado en una URL pública HTTPS. WhatsApp puede tardar en actualizar la vista previa y puede conservar una miniatura anterior en caché. La imagen OG usa una ruta relativa; para máxima compatibilidad con todos los rastreadores, después de publicar reemplazá `assets/whatsapp-preview.jpg` en `og:image` y `twitter:image` por la URL absoluta de esa imagen, por ejemplo:
`https://TU-USUARIO.github.io/TU-REPOSITORIO/assets/whatsapp-preview.jpg`

## Nota
La instalación PWA requiere HTTPS (GitHub Pages lo proporciona). Los cambios al juego deben probarse en navegador de escritorio y en un teléfono real.
