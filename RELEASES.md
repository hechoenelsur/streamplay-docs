# 📦 Release Notes Extendidas - StreamPlay WP

## ✅ v2.1.9e
Play en uno ejecuta Stop real en los otros, garantizando corte total del stream y evitando consumo de datos innecesario.

## ✅ v2.1.9d
Usa lista interna robusta de reproductores Plyr para garantizar que al presionar Play en uno, todos los demás se pausen correctamente, incluso después de reconstrucciones.

## ✅ v2.1.9c
Stop reconstruye sin autoplay, dejando esperar al usuario. Al presionar Play en uno, pausa automáticamente otros activos.

## ✅ v2.1.9b
Reconstrucción tras Stop con activación automática de Play (rollbackado luego por problemas de exclusividad).

## ✅ v2.1.9
El botón Stop se coloca alineado al lado derecho del Play/Pause, y se fuerza actualización del CSS para evitar problemas de cache.

## ✅ v2.1.8
Stop destruye y reconstruye completamente el reproductor, garantizando reconexión limpia al volver a Play.

## ✅ v2.1.7
Introducción del botón Stop manual. Se intentó controlar la pausa real del streaming para evitar buffering residual.


# 📦 Release Notes Extendidas - Parte 2 - StreamPlay WP

## ✅ v2.1.6
Ajustes visuales en el botón Stop y mejora en el control del stream al usar Play/Pause.

## ✅ v2.1.5
Sistema de exclusividad: solo un reproductor puede sonar a la vez. Cuando presionas Play en uno, el otro se pausa automáticamente.

## ✅ v2.1.2
Se integra completamente Plyr.js para mejorar el diseño visual y la interacción con los reproductores.

## ✅ v2.1.1
Retorno al uso de admin-ajax.php para scrapear los títulos dinámicamente, con integración completa de Plyr.js.

## ✅ v2.1.0
Primera integración de Plyr.js + sistema de consulta usando proxy.php (reversión en versiones siguientes).

## ✅ v2.0.0
Refactorización mayor del plugin. Se eliminó la dependencia de `proxy.php` y se pasó a reproducir directamente los streams.

## ✅ v1.2.1
Se implementa `admin-ajax.php` como mecanismo para obtener dinámicamente el título de la canción en reproducción.

## ✅ v1.0.0
Primera versión pública y estable del plugin. Incluye dos reproductores con streams directos.
