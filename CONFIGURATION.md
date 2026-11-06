# ZoneProtes — Configuration / Configuración (2026-11-06)

| Side / Lado | Version / Versión |
|---|---|
| Server / Servidor | 2.11.1 |
| Client / Cliente — retained / conservado | 2.10.4 |

## Staff permissions / Permisos de staff

| Node / Nodo | Access / Acceso |
|---|---|
| `zonaprotes.claim.view` | Inspect any known player's claims, including offline, with names/coordinates/pages; no travel / Consultar cualquier dueño conocido, incluso desconectado, sin viajar |
| `zonaprotes.claim.teleport` | Inspect and travel to any player's claims / Consultar y viajar |
| `zonaprotes.admin` | Existing full administration, including inspection/travel / Administración anterior completa |

The two new nodes default to denied. OP2+ retains access. Use ZoneRanks or a compatible Forge permission provider. If a player still has `zonaprotes.admin` or OP, assigning only the view node does not remove their broader travel access. / Los nuevos nodos vienen denegados; OP2 conserva acceso. Asignar view no retira administración/OP existentes.

These nodes do not grant building, container access, anchor removal or other players' flag management. Visiting does not grant editing rights. / No conceden construcción, cofres, retirada de anclas ni gestión ajena de flags.

## Commands / Comandos

```text
/protes ver NombreJugador
/protes ver NombreJugador pagina 2
/protes ver NombreJugador 1
```

`/prote` is an alias. Known names and UUIDs are accepted without remote name lookup. The final numeric form selects according to the current list; [IR] buttons instead retain the region anchor. / Alias `/prote`; nombres conocidos/UUID sin búsquedas remotas. El número escrito usa lista actual, mientras [IR] conserva ancla.

Permissions are rechecked at execution, including previously parsed commands. Command suggestions may require the provider to refresh or reconnect, but server validation remains authoritative. / Permisos se comprueban al ejecutar; sugerencias pueden necesitar refresco o reconexión sin sustituir validación.

## Update continuity / Continuidad

Keep the world, protection/member/flag data, messages and current TOML. Replace only the server JAR with2.11.1; client 2.10.4 and protocol split-1 remain. `/reload` cannot load a new JAR. No new TOML key is needed for these staff permission nodes. / Conserva datos/configuración; solo cambia servidor. `/reload` no carga JAR nuevo; los permisos nuevos no requieren claves TOML nuevas.

[Current release / Entrega actual](RELEASE-2026-11-06.md) · [README](README.md).
