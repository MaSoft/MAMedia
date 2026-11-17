# MAMedia

Reproductor de vídeo y música para el móvil: biblioteca con lo que ya hay en el teléfono, favoritos, listas y «seguir donde lo dejaste», con zoom y gestos en el vídeo, subtítulos y ecualizador. Funciona sola, sin PC.

**Aplicación gratuita para Android desarrollada por [Masoft.es](https://masoft.es)**

[![Descargar](https://img.shields.io/github/v/release/MaSoft/MAMedia?label=Descargar&style=for-the-badge)](https://github.com/MaSoft/MAMedia/releases/latest)

Más información y el manual también en [masoft.es](https://masoft.es/android.html#mamedia).

![Biblioteca y carpetas](capturas/01-biblioteca.webp)

## Características
- Biblioteca de vídeos, música, carpetas y recientes del móvil, sin buscar carpetas, con buscar y ordenar.
- Carpetas del móvil en árbol (memoria interna y tarjeta SD) con filtro de vídeo o música.
- Reproductor a pantalla completa con gestos: doble toque para avanzar o retroceder, deslizar para buscar, brillo y volumen.
- Zoom hasta 8× sin parar el vídeo, con minimapa, fotograma a fotograma y captura del fotograma.
- Subtítulos del vídeo y .srt, .vtt o .ass de su carpeta, pista de audio, velocidad de 0,25× a 3× y repetición A-B.
- Favoritos, listas que se ordenan arrastrando, importación y exportación de listas .m3u, y cola de reproducción.
- Música con ecualizador y preajustes, mandos en la notificación y en la pantalla de bloqueo, segundo plano e imagen en imagen.
- Abre los vídeos y la música que se comparten desde otras apps y sigue con el resto de la carpeta en orden.
- Botones de la barra del reproductor a tu gusto: cuáles se ven y en qué orden.

## Capturas

| | |
|---|---|
| ![Música](capturas/02-musica.webp)<br>**Música.** Canciones del móvil y reproductor de música con favoritos, cola, velocidad y repetición A-B. | ![Favoritos y listas](capturas/03-listas.webp)<br>**Favoritos y listas.** Favoritos de vídeo y música y listas propias que se ordenan arrastrando. |
| ![Reproductor y ecualizador](capturas/04-reproductor.webp)<br>**Reproductor y ecualizador.** Reproductor de vídeo con «seguir donde lo dejaste» y ecualizador de 10 bandas con preajustes. |  |

## Requisitos

| | |
|---|---|
| Sistema | Android 11 o superior |
| Permisos | Fotos y vídeos y Música y audio para ver tu biblioteca; notificaciones para los mandos; acceso a todos los archivos solo para mover archivos y leer los subtítulos de la carpeta. |
| Instalación | Se descarga el APK en el móvil y se abre; Android pide permiso para instalar aplicaciones de esa fuente. |
| Actualizar | La versión nueva se instala encima de la anterior sin perder nada. |

Funciona sola en el móvil. La sincronización con MAMedia de escritorio, que el manual explica (capítulo 6), es opcional y esa versión no se publica. El manual es común al PC y al móvil: la app Android está en su capítulo 6.

## Descarga y comprobación

En [Releases](https://github.com/MaSoft/MAMedia/releases/latest) están la aplicación (`MAMedia-1.3.0.apk`), su huella SHA-256 y el manual. Las aplicaciones no están en Google Play: se instalan desde el APK y Google Play Protect puede avisar de que no conoce la aplicación.

Para comprobar que la descarga está completa, en PowerShell:

```powershell
Get-FileHash .\MAMedia-1.3.0.apk
```

Debe coincidir con `238f08a8fdc4e92e17f210d04f44e3cab15e5eefae35d8be498693cfc551a46f`.

## Manual

[manual_MAMedia.html](https://github.com/MaSoft/MAMedia/releases/latest/download/manual_MAMedia.html): descárgalo y ábrelo en el navegador.

## Aviso legal

MAMedia es gratuito y se entrega tal cual, sin garantía de ningún tipo. Al descargarlo y usarlo aceptas el aviso legal y las limitaciones de su manual.

> ⚠ MAMedia reproduce los archivos que tú tienes; no descarga ni desbloquea nada. Las capturas de fotograma de películas, series o vídeos de otras personas están sujetas a sus derechos de autor y de imagen: úsalas solo para fines personales o permitidos por la ley. «Mover a carpeta» mueve archivos de verdad: comprueba el destino antes de aceptar.

**Limitaciones y exclusión de responsabilidad**
- Los vídeos con protección anticopia (DRM, como los de plataformas de pago) no se pueden reproducir.
- Favoritos, listas y posiciones se guardan en los datos de la app (Android no deja leerlos a otras apps), sin cifrar aparte.
- La app usa ExoPlayer (AndroidX Media3, licencia Apache 2.0) y los códecs del propio móvil: lo que el móvil no sabe decodificar (por ejemplo DTS en muchos modelos) no suena, aunque el vídeo se vea.
- MAMedia se proporciona tal cual, sin garantía de ningún tipo.

Este repositorio solo contiene la aplicación compilada y su documentación. © Masoft.es. Todos los derechos reservados.
