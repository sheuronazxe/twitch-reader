# Twitch Reader

Text-to-Speech inteligente para leer mensajes de tu chat de Twitch en voz alta.

## Características

- **Conexión IRC** — Se conecta directamente al chat de Twitch via WebSocket
- **Text-to-Speech** — Lee los mensajes en voz alta usando la API de Web Speech del navegador
- **Filtros avanzados** — Blacklist, whitelist, ignorar URLs, emotes, comandos
- **Modo donaciones** — Lee solo mensajes con bits que superen un mínimo configurable
- **Roles de Twitch** — Configurable por rol: Streamer, Mods, VIPs, Subs
- **Motor de Audio** — Selecciona voz, volumen, velocidad y tono
- **Temas claro/oscuro**
- **Persistencia** — Guarda configuración en LocalStorage
- **Exportar/Importar** — Configuración en JSON

## Uso

1. Abre `index.html` en tu navegador (preferiblemente Chrome o Edge para mejor calidad de TTS)
2. Escribe el nombre de tu canal de Twitch y pulsa **Conectar**
3. Los mensajes del chat se leerán automáticamente

## Atajos de teclado

| Tecla | Acción |
|------|--------|
| `ESC` | Limpiar cola |
| `SPACE` | Saltar mensaje actual |

## Configuración

- **Volumen** — Ajusta el volumen de salida (0-100%)
- **Velocidad** — Velocidad del habla (0.5x - 2x)
- **Tono** — Tono de la voz (0.5 - 2)
- **Pausa entre mensajes** — Retardo entre mensajes en cola (0-3000ms)

## Permisos por rol

En la sección *Filtros y Reglas*, activa **Siempre leer a** para que un rol ignore todos los filtros:

- **Streamer** — El dueño del canal
- **Moderadores** — Usuarios con rol de mod
- **VIPs** — Usuarios VIP
- **Subs** — Suscriptores

## Formato de voz

- Donaciones de bits: `"Nombre envió X bits: mensaje"`
- Mensajes normales: `"Nombre dice: mensaje"`

## Notas

- Requiere conexión HTTPS para usar WebSocket en producción
- Algunas voces en español necesitan instalación en el sistema operativo
- La configuración se guarda automáticamente en el navegador

## Autor

Creado por @sheuronazxe