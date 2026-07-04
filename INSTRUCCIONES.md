# Plantilla Elegante — Instrucciones rápidas

## 1. Falta el video
Copia tu video actual (el que ya usas en la Romántica) a:
```
img/video-intro.mp4
```
Si no lo pones, el sitio funciona igual pero salta directo a la invitación al tocar el sello.

## 2. Conectar Airtable (libro de firmas)
En `js/config.js`, sección `airtable`, pega:
- `apiKey`: tu API key de Airtable
- `baseId`: el ID de tu base
- `tableId`: normalmente "Firmas"

Puedes usar las mismas credenciales de tu invitación actual para probar.

## 3. Conectar Cloudinary (galería)
En `js/config.js`, sección `cloudinary`, pega:
- `cloudName`
- `uploadPreset`

Mismas credenciales que ya usas también sirven para probar.

## 4. Editar contenido
Todo el contenido (nombres, fecha, mensajes, historia, timeline) está en `js/config.js`.
No hay que tocar `index.html`, `style.css` ni `main.js` para cambiar textos — solo edita los arrays.

Para agregar/quitar un mensaje, un párrafo de historia, o un evento del timeline: copia o borra un bloque `{ ... }` dentro del array correspondiente.

## 5. Subir a GitHub Pages
1. Crea un repositorio (o usa uno existente)
2. Sube esta carpeta completa (`index.html`, `css/`, `js/`, `img/`)
3. Settings → Pages → activa GitHub Pages en la rama `main`
4. Tu link estará disponible en 2-3 minutos

## 6. Fotos de la historia
Agrega tus fotos reales en `img/historia/` con los nombres que están en `config.js`
(`foto1.jpg`, `foto2.jpg`, etc.) o cambia los nombres en el config.
