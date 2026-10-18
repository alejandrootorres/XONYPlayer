# XONY Player — Android starter project

Proyecto Android nativo en Kotlin con interfaz negra/violeta/cian, selector de audio local y reproducción de enlaces directos HTTPS.

## Requisitos
- Android Studio/Gradle en un entorno de compilación, o GitHub Actions desde el navegador.
- Java 17 y Gradle 8.9 (el workflow de GitHub los configura automáticamente).

## Compilar gratis desde el celular con GitHub Actions
1. Descarga y descomprime este ZIP.
2. En el navegador del teléfono abre https://github.com/ y crea un repositorio nuevo llamado `XONYPlayer`. Déjalo vacío (sin README).
3. Sube los archivos y carpetas de este proyecto al repositorio. GitHub móvil puede ser incómodo para carpetas; si no te permite subir carpetas, usa la vista de escritorio del navegador o la app de GitHub si está disponible.
4. Abre la pestaña **Actions** del repositorio. Si GitHub te pide habilitar workflows, acepta.
5. El workflow `Build XONY Player APK` se ejecuta al subir a `main`. También puedes abrirlo y tocar **Run workflow**.
6. Cuando termine en verde, abre la ejecución y baja a **Artifacts**. Descarga `XONY-Player-debug`.
7. Descomprime el artifact ZIP y abre `app-debug.apk` en tu teléfono para instalarlo. Android podría pedirte permitir instalar aplicaciones desde el navegador o administrador de archivos.

## Prueba de streaming
Usa un enlace HTTPS directo a un archivo o stream de audio compatible. Un enlace a una página de YouTube, Spotify, SoundCloud u otra web normalmente no es un enlace de audio directo.

## Alcance de esta versión
- Selección de un archivo de audio mediante el selector de Android.
- Reproducción local y streaming HTTPS con MediaPlayer.
- Botones de reproducir/pausar y volver al inicio de la pista.
- Interfaz inicial adaptada a móvil.

Todavía no incluye reproducción en segundo plano mediante servicio, notificación multimedia, cola automática de canciones, escaneo completo de biblioteca, favoritos persistentes ni listas guardadas. El control de progreso está visualmente preparado, pero aún no está sincronizado con la duración real. Esta es una base funcional inicial, no una app publicada ni probada en todos los dispositivos.
