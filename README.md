# MineNovate Bot

Bot de Discord en JavaScript (Node.js 20 + discord.js 14), con comandos slash globales y configuración independiente por servidor.

## Instalación
1. Instala Node.js 20 o superior.
2. Ejecuta `npm install`.
3. Copia `.env.example` a `.env` y completa DISCORD_TOKEN y CLIENT_ID.
4. Activa **Server Members Intent** en Discord Developer Portal.
5. Ejecuta `npm run deploy` una vez y luego `npm start`.

## Comandos
- `/config bienvenida|despedida|logs|categoria-tickets|soporte|ver`
- `/ticket crear|cerrar`
- `/help`, `/ping`, `/serverinfo`
- Moderación: `/warn`, `/timeout`, `/kick`, `/ban`, `/clear`
- Economía: `/balance`, `/daily`, `/work`, `/pay`, `/leaderboard`

Los ajustes de canales/roles se guardan por ID de servidor en data/guilds.json. La economía se guarda por servidor en data/economy.json. En hosting con almacenamiento efímero, configura disco persistente o una base de datos externa.

**Seguridad:** nunca subas el archivo .env ni compartas tu token. Los comandos globales pueden tardar en propagarse.
