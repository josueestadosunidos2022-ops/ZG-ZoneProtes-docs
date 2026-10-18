# ZoneProtes — TOML configuration reference

This guide describes **server 2.9.1 / client 2.9.1**. ForgeConfigSpec keys below are literal source defaults. The server generates the final TOML. Never commit real world data or server secrets. / Esta guía corresponde a **servidor 2.9.1 / cliente 2.9.1**. Las claves siguientes son los valores iniciales declarados; el servidor genera el TOML definitivo. Nunca publiques datos reales del mundo o secretos.

## Configuration files

- `config/zonaprotes/protecciones.toml`: ordered editable protection catalog / catálogo ordenado editable.
- `config/zonaprotes-common.toml`: Forge global protection, terrain, messages and antiDupe switches / opciones globales Forge.
- `config/zonaprotes/protecciones/creadas.toml`: informational export of created claims; persistent claims live in world saved data `protes_claims` / exportación informativa; la persistencia real está en datos del mundo.

## Detected keys / Claves detectadas

| Key / Clave | Declared default | Source class |
|---|---|---|
| `announceRegions` | `true` | `ZonaProtesConfig.java` |
| `blockAutomation` | `true` | `ZonaProtesConfig.java` |
| `blockAutomationCapabilities` | `false` | `ZonaProtesConfig.java` |
| `blockAutomationStrict` | `false` | `ZonaProtesConfig.java` |
| `blockExplosions` | `true` | `ZonaProtesConfig.java` |
| `blockFallingBlockPortals` | `true` | `ZonaProtesConfig.java` |
| `blockFire` | `true` | `ZonaProtesConfig.java` |
| `blockFluidFlow` | `true` | `ZonaProtesConfig.java` |
| `blockHostileSpawning` | `false` | `ZonaProtesConfig.java` |
| `blockMobGriefing` | `true` | `ZonaProtesConfig.java` |
| `blockPistons` | `true` | `ZonaProtesConfig.java` |
| `blockRiskyPistonMoves` | `true` | `ZonaProtesConfig.java` |
| `blockUnattributedBlockChanges` | `true` | `ZonaProtesConfig.java` |
| `protectContainers` | `true` | `ZonaProtesConfig.java` |
| `protectDroppedItems` | `true` | `ZonaProtesConfig.java` |
| `protectEntities` | `true` | `ZonaProtesConfig.java` |
| `validateFallingSource` | `true` | `ZonaProtesConfig.java` |
| `validateOpenContainers` | `true` | `ZonaProtesConfig.java` |

## Catalog / Catálogo

Each `[[protecciones]]` entry accepts `id`, `nombre`, `tamano` (integer 1–512), `textura` (one of coal, iron, diamond, emerald, amethyst, gold, netherite), `subtitulo`, `estatus` and `descripcion` (text list). Default sizes in order are 9, 16, 26, 56, 100, 150 and 220. `tamano` is the number of blocks from the anchor in **each** X/Z direction; height is unlimited. Existing claims keep their saved size until explicit synchronization. Text supports `{medidas}`, `{tamano}` and `{id}`. Reload via `/protes reload`. / Cada entrada admite esas claves; `tamano` es el alcance desde el ancla hacia **cada** dirección X/Z, con altura ilimitada. Las protecciones existentes mantienen su tamaño guardado hasta sincronizarlas. Las variables de texto son `{medidas}`, `{tamano}` y `{id}`.

## Commands and permissions / Comandos y permisos

- `/protes tipos`, `/protes dar`, `/protes crear`, `/protes textura`, `/protes tamano`, `/protes reload`, `/protes lista`, `/protes sincronizar [confirmar]`, `/protes editar abrir|cerrar`: administrator tools, permission `zonaprotes.admin` or OP level 2 / herramientas de administrador.
- `/protes ver <nombre|UUID>`: administrator list and safe travel by claim number / lista y viaje seguro por número para administradores.
- `/protes aqui`, `/protes permisos`, `/protes permiso <jugador> permitir|denegar|heredar`, `/protes maquinas permitir|bloquear`: location, current claim access and audited machine policy / ubicación, acceso local y máquinas auditadas.
- `/protes invitar|expulsar|miembros|promote|degradar|cosduenos`: team management, permission `zonaprotes.team.manage`; placing claims uses `zonaprotes.claim.create`. The latter two default to allowed by Forge permission fallback, while admin defaults to OP only / gestión de equipo; estos dos permisos se permiten por defecto, admin solo OP.

`blockAutomationCapabilities=false` and `blockAutomationStrict=false` are deliberate interoperability defaults. Turning either on can stop storage or machines even for owners. `blockHostileSpawning=false` is also deliberate. / Esos dos bloqueos estrictos están apagados para conservar almacenaje y máquinas incluso del dueño. La aparición hostil también permanece habilitada por defecto.

