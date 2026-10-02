# EnVoIP Phone

Softphone SIP moderno para **Windows, macOS, Android e iOS**, pensado para usarse con
**Vicidial / ViciBox** y cualquier servidor SIP con WebSocket (Asterisk, FreeSWITCH, Kamailio…).

Parte de **[EnVoip System](https://github.com/retsill/envoip-system)** · © 2006 - 2026 · Worked: [XcoDevs](https://xcodevs.com) · by: [Enwebs Estudios](https://enwebs.net)

## Descargar para Windows

1. Ve a **[Releases](../../releases/latest)** y descarga **`EnVoIP-Phone-Setup-X.Y.Z.exe`**.
2. Ejecútalo y sigue el asistente. No necesita permisos de administrador ni instalar nada más
   (incluye el runtime de Visual C++). Si Windows SmartScreen avisa («Windows protegió su PC»), pulsa
   **Más información → Ejecutar de todas formas** (la app aún no está firmada digitalmente).
3. Abre **EnVoIP Phone** desde el menú Inicio o el escritorio. Se desinstala desde *Configuración → Aplicaciones*.
4. La primera llamada pedirá permiso para el **micrófono**.

También está la versión portable `EnVoIP-Phone-Windows-vX.Y.Z.zip`: descomprímela y ejecuta `envoip_phone.exe`.

## Descargar para macOS

1. En **[Releases](../../releases/latest)** descarga **`EnVoIP-Phone-X.Y.Z.dmg`** (Intel y Apple Silicon, macOS 10.15 o superior).
2. Ábrelo y arrastra **EnVoIP Phone** a la carpeta **Aplicaciones**.
3. La primera vez: clic derecho sobre la app → **Abrir** → **Abrir** (la app aún no está firmada con un
   Developer ID de Apple). Si macOS no ofrece «Abrir»: *Ajustes del Sistema → Privacidad y seguridad →
   Abrir igualmente*.
4. La primera llamada pedirá permiso para el **micrófono**.

## Descargar para Android y Chromebook

1. En **[Releases](https://github.com/retsill/envoip-phone-releases/releases/latest)** descarga **`EnVoIP-Phone-X.Y.Z.apk`**
   (Android 7.0 o superior; Chromebooks Intel/AMD y ARM).
2. **Android:** ábrelo desde Descargas y permite «Instalar apps desconocidas» para el navegador o el gestor de archivos.
3. **Chromebook:** Google Play debe estar activado. Abre el `.apk` desde la app *Archivos*. Si ChromeOS no ofrece
   instalarlo, actívalo en *Configuración → Acerca de ChromeOS → Desarrolladores → Entorno de desarrollo de Linux →
   Desarrollar apps para Android → Habilitar la depuración de ADB*, y luego en la terminal de Linux:
   `sudo apt install -y adb && adb connect arc && adb install EnVoIP-Phone-X.Y.Z.apk`.
4. La primera llamada pedirá permiso para el **micrófono**.

## Primeros pasos

- **Líneas** (Ajustes → Líneas → Añadir → *Vicidial / ViciBox*): IP o dominio del servidor, la extensión y su
  *Registration Password*. Con ViciBox recién instalado, deja activado «Aceptar certificados autofirmados».
- **Mensajes (SMS/MMS)**: en la línea, sección *Mensajes*, elige **Servidor EnVoip System** y entra con tu usuario de
  Vicidial (comparte las conversaciones con la web), o la **API de VoIP.ms**, o **SIP MESSAGE**.
- **Vista compacta / ampliada**: botón ⤢ en el teclado (escritorio).

## Funciones

- Varias líneas SIP sobre WebSocket seguro (WSS) con audio WebRTC cifrado.
- Llamadas: marcar, contestar/rechazar, silencio, espera, DTMF, transferir, varias llamadas, tono de espera.
- Contactos locales con favoritos y búsqueda.
- SMS/MMS: servidor EnVoip System, API de VoIP.ms o SIP MESSAGE.
- Historial, selección de micrófono y altavoz, tema claro/oscuro, inglés y español.

## Versiones

Todas las versiones publicadas están en **[Releases](../../releases)**. Este repositorio solo contiene las
aplicaciones compiladas; el código fuente de la app es privado.
