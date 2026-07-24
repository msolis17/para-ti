# Viaje El Salvador

Página romántica con:
- Candado (clave `1608`)
- Contador al viaje (30 jul 2026)
- Contador al cumpleaños (16 ago) + mensaje desde el **6 ago**
- Misiones por día (se desbloquean por fecha; solo lectura, sin checks)
- Álbum secreto (se abre el **3 ago**)

## Cómo personalizar

En `index.html`, objeto `CONFIG`:
- `clave`, fechas, mensajes
- `dias` → misiones
- `album` → después del viaje agrega fotos:

```js
album: [
  { src: 'fotos/dia1-selfie.jpg', caption: 'Día 1' },
  { src: 'fotos/skydeck.jpg', caption: 'Skydeck' },
],
```

## Subir a un repo nuevo (GitHub Pages)

1. Crea un repo nuevo en GitHub (ej. `ViajeElSalvador`).
2. Sube `index.html` + carpeta `fotos/`.
3. Settings → Pages → **Deploy from a branch** → `main` → `/ (root)`.
4. Link: `https://TU_USUARIO.github.io/ViajeElSalvador/`

## Notas

- Las fotos **no** se suben solas desde la web: tú las agregas a `fotos/` y actualizas `CONFIG.album`.
- El desbloqueo del candado sí usa localStorage en el celular.
