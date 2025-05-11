# Changelog StreamPlay WP
***************

## [2.1.9e] (2025-05-08 18:40 UTC-3)
Play en uno ejecuta Stop real en los otros, garantizando corte total del stream y evitando consumo de datos innecesario.

## [2.1.9d] (2025-05-08 18:10 UTC-3)
Usa lista interna robusta de reproductores Plyr para garantizar que al presionar Play en uno, todos los demás se pausen correctamente, incluso después de reconstrucciones.

## [2.1.9c] (2025-05-08 17:40 UTC-3)
Stop reconstruye sin autoplay, dejando esperar al usuario. Al presionar Play en uno, pausa automáticamente otros activos.

## [2.1.9b] (2025-05-08 17:10 UTC-3)
Reconstrucción tras Stop con activación automática de Play (rollbackado luego por problemas de exclusividad).
Al reconstruir tras Stop, asegura que Play funcione de inmediato sin doble clic.

- Stop reconstruye sin autoplay, esperando al usuario.
- Play pausa automáticamente otros streams activos.

## [2.1.9] (2025-05-08 16:40 UTC-3)
El botón Stop se coloca alineado al lado derecho del Play/Pause, y se fuerza actualización del CSS para evitar problemas de cache.
- Botón Stop visualmente alineado.
- Cache de CSS forzado a actualizar.

## [2.1.8]
Stop destruye y reconstruye completamente el reproductor, garantizando reconexión limpia al volver a Play.

## [2.1.7]
Introducción del botón Stop manual. Se intentó controlar la pausa real del streaming para evitar buffering residual. Refinamientos visuales.
Al presionar Pause corta la conexión del stream; Play reconecta automáticamente

## [2.1.6]
Ajustes de compatibilidad y refinamiento visual en el botón Stop y el control de streams.

## [2.1.5]
Implementación del sistema de exclusividad: al presionar Play en un reproductor, pausa el otro. Mejora de la interfaz responsive.

## [2.1.2]
Integración completa de estilo Plyr, mejora de los estados de play/pause y solución a bugs de visualización.

## [2.1.1]
Retorno al scrap por admin-ajax.php para mostrar títulos dinámicos + integración estable con Plyr.js.

## [2.1.0]
Integración inicial de Plyr.js, control visual avanzado y consulta usando nuevamente proxy.php

## [2.0.0]
Refactorización mayor para quitar dependencias de proxy.php, usando solo streams directos.

## [1.2.1]
Usa admin-ajax.php para scrapear títulos dinámicamente.

## [1.0.0]
Primera versión estable (básica), con reproductores funcionales cargando streams directos.
