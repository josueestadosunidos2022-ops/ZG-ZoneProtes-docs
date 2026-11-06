# ZoneProtes

Player-owned protection regions with members, flags and administrative claim inspection.

Regiones protegidas de jugadores con miembros, flags y consulta administrativa de protecciones.

## Current release / Entrega actual — 2026-11-06

Minecraft **1.20.1**, Forge **47.x** (47.4.x for this release set), Java **17**. File availability follows CurseForge approval. / Disponibilidad de archivos según aprobación de CurseForge.

| Side / Lado | Version / Versión |
|---|---|
| Server / Servidor | 2.11.1 |
| Client / Cliente — retained / conservado | 2.10.4 |

**Protocol / Protocolo:** split-1.

[Downloads / Descargas](https://www.curseforge.com/projects/1738057/files) · [Release guide / Guía de novedades](RELEASE-2026-11-06.md) · [Configuration / Configuración](CONFIGURATION.md)

## English — Requirements and quick start

Server: ZoneCore 2.1.3+. Keep the compatible client 2.10.4. Optional ZoneRanks or a Forge permission provider can assign the new staff nodes; no client update is required.

Staff use `/protes ver NombreJugador`, `/protes ver NombreJugador pagina 2` and permitted [IR] buttons. `/prote` remains an alias. Grant view-only access without admin/OP if travel must remain unavailable.

### What changed

- Separate staff permission nodes for inspecting claims and for visiting them, including known offline owners.
- Travel buttons target owner/dimension/anchor instead of a changing list position; permissions are checked again on execution.
- Safe destinations consider standing/current body dimensions. Successful travel clears fall/velocity; cancelled or failed travel reports failure and retains previous state.

## Español — Requisitos e inicio

Servidor: ZoneCore 2.1.3+. Conserva cliente 2.10.4 compatible. ZoneRanks u otro proveedor Forge puede asignar permisos nuevos; no hace falta actualizar cliente.

Staff usa `/protes ver NombreJugador`, `/protes ver NombreJugador pagina 2` y [IR] permitido. `/prote` sigue como alias. Para solo consulta, evita conceder también administración/OP que habilite viaje.

### Novedades

- Permisos separados para consultar protecciones y visitarlas, incluyendo dueños desconectados conocidos.
- Botones de viaje asociados a dueño/dimensión/ancla en vez del orden variable; permisos validados al ejecutar.
- Destino seguro considera cuerpo de pie/actual. Viaje logrado limpia caída/velocidad; cancelado o fallido informa y conserva estado.

## Updating / Actualizar

Stop the affected instance, back up world/configuration, replace only the previous same-mod/same-side JAR and retain player data. Never install the dedicated and client JARs of one mod together. / Detén la instancia correspondiente, respalda mundo/configuración y sustituye solo el JAR del mismo mod y lado conservando datos. Nunca instales juntos los JAR dedicado y cliente del mismo mod.

## Validation scope / Alcance de verificación

The release includes targeted permission and teleport regression evidence. It does not certify arbitrary modded hazards, every machine integration or a production multiplayer deployment.

La entrega incluye evidencia acotada de permisos y teletransporte. No certifica peligros arbitrarios de otros mods, todas las máquinas ni despliegue multijugador de producción.

## Rights / Derechos

Original ZONE code and assets © Elgochogms; existing licenses and third-party notices remain applicable. This repository provides public documentation. / Código y recursos originales ZONE © Elgochogms; se conservan licencias y avisos de terceros. Este repositorio contiene documentación pública.
