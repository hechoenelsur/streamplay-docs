# 🧱 Arquitectura - StreamPlay WP

## 🧩 Componentes principales

- `streamplay.php`: plugin base, define el shortcode `[streamplay]`.
- Plyr.js: reproductor moderno y ligero con controles extendidos.
- `admin-ajax.php`: se usa para scrapear metadatos (título de canción).
- JavaScript personalizado: gestiona exclusividad, toggle mobile, marquesina y reconexión.

## 🔄 Flujo de reproducción

1. Se genera el HTML de dos reproductores con IDs únicos.
2. Se aplica Plyr.js sobre cada uno.
3. Cada 15 segundos se hace fetch a `admin-ajax.php` para actualizar el título de la canción.
4. Al presionar Play en uno, el otro se detiene (Stop real).
5. Al presionar Stop, se reconstruye el reproductor para asegurar reconexión limpia.

## 📱 Compatibilidad
- Totalmente responsive.
- Toggle automático para minimizar reproductores en mobile.

## 🧠 Lógica de Exclusividad
- Cada reproductor registrado en un array global.
- Al presionar Play, todos los demás son detenidos (`stop()` y `destroy()`).
