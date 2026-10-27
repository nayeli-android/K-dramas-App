# Revisión de KDrama v1.1.0

Evaluación realizada el 21 de octubre de 2026 en un Samsung SM-S948B con Android 17. El instalador probado fue `KDrama-App-v1.1.0.apk`. La versión `v1.2` requiere una nueva prueba para confirmar cuáles hallazgos siguen vigentes.

| Hallazgo | Pasos para reproducir | Resultado esperado | Resultado observado en v1.1.0 |
| --- | --- | --- | --- |
| La sesión no se restaura al reabrir | Iniciar sesión, cerrar la app por completo y volver a abrirla. | Abrir la pantalla principal mientras la sesión siga vigente. | Vuelve a mostrar el inicio de sesión. Se reprodujo dos veces. |
| La versión interna no coincide con la publicación | Instalar el APK de `v1.1.0` y consultar los metadatos del paquete en Android. | Android identifica la compilación como `1.1.0`. | `versionName` es `1.0.0` y `versionCode` es `1`. |
| El catálogo queda en blanco | Iniciar sesión, abrir Inicio, esperar la carga y alternar entre Todos y Romance. | Mostrar títulos o explicar que no hay contenido o que falló la carga, con opción de reintentar cuando corresponda. | Bajo “Catálogo Completo” no aparecen tarjetas ni mensaje. No se pudo distinguir entre ausencia de datos y fallo de consulta. |
| Los avisos contradicen Mi Lista | Iniciar sesión, abrir la campana, leer el aviso de un episodio añadido y abrir Mi Lista. | Mostrar avisos correspondientes a los eventos y el contenido de la cuenta. | Aparecen dos avisos predeterminados, incluido el del episodio añadido, mientras Mi Lista está vacía. |

También se abrieron Inicio, Mi Lista, Perfil y los formularios de nombre y contraseña, sin guardar cambios. Como el catálogo no mostró títulos, no se pudo revisar la ficha de un drama, la reproducción de episodios ni el agregado a Mi Lista. No se publicó contenido desde la app.
