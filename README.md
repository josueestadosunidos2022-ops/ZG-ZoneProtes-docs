# ZG ZoneProtes

## Update / Actualización — 2026-10-17

Selected version / Versión seleccionada: **server 2.10.4 / client 2.10.4**. New file availability depends on CurseForge approval / La disponibilidad de los archivos nuevos depende de su aprobación en CurseForge.

See [changes, exact files and installation](UPDATES-2026-10-17.md) / Consulta [cambios, archivos e instalación](UPDATES-2026-10-17.md). Preserve the world and TOML files / Conserva mundo y TOML.

## English

Vertical land protection enforced by the server, with seven original ZG block designs, team access, a TOML catalog, automation border checks and anti dupe guards. For Minecraft 1.20.1, Forge 47.x, Java 17.

### Installation

Install zonaprotes-server-2.10.4-protected.jar and ZG ZoneCore 2.1.3 or newer on the dedicated server. Install zonaprotes-client-2.10.4-protected.jar on each player's client. The two JARs belong to this one CurseForge project; install only the file for each side. Both use protocol split-1. The client contains visuals and minimal registry, while the server enforces claims. Back up the world and config/zonaprotes before updating.

### Features

- A configured protection block covers the whole world height. The TOML size is the reach in each horizontal direction from the anchor: size 26 reaches 26 blocks on every side.
- Owners can invite members, promote co owners, set local player access and allow or block audited machines in their claim. Only owners, co owners and staff may remove the anchor.
- /protes ver <name|UUID> lists claims and /protes ver <name|UUID> <number> travels to a safe point near one. Administrators can reload and synchronize the catalog.
- ZoneClans wars, ZoneMap overlays, ZoneEssentials rollback and ZoneLevelUp arena checks use public claim interfaces. Create fixed machinery, Botania fluid consumers and DivineRPG Rive have optional guards. Mobile Create contraptions are not authorized by the fixed machine rule.

Read [TOML configuration and commands](CONFIGURATION.md) and [release compatibility](RELEASES.md). Strict automation switches may break storage even for the owner; a full third party modpack needs its own tests.

## Español

Protecciones verticales aplicadas por el servidor, con siete diseños ZG originales, acceso por equipo, catálogo TOML, control en fronteras de automatización y defensas contra duplicación. Para Minecraft 1.20.1, Forge 47.x, Java 17.

### Instalación

Instala zonaprotes-server-2.10.4-protected.jar y ZG ZoneCore 2.1.3 o posterior en el servidor dedicado. Instala zonaprotes-client-2.10.4-protected.jar en cada cliente. Ambos JAR pertenecen a este único proyecto CurseForge; instala solo el archivo de cada lado. Ambos usan el protocolo split-1. El cliente contiene recursos visuales y registro mínimo; el servidor aplica las protecciones. Respalda el mundo y config/zonaprotes antes de actualizar.

### Funciones

- El bloque protege toda la altura del mundo. El tamaño TOML es el alcance horizontal desde el ancla en cada dirección: 26 alcanza 26 bloques por cada lado.
- El dueño invita miembros, asciende codueños y establece acceso local y permisos de máquinas auditadas. Solo dueño, codueños y personal pueden retirar el ancla.
- /protes ver <nombre|UUID> lista protecciones y /protes ver <nombre|UUID> <numero> viaja a una posición segura próxima. El administrador puede recargar y sincronizar el catálogo.
- ZoneClans, ZoneMap, ZoneEssentials y ZoneLevelUp usan interfaces públicas. Las máquinas fijas Create, consumidores de fluidos Botania y Rive de DivineRPG tienen controles opcionales. La regla de máquina fija no autoriza contraptions móviles de Create.

Consulta [configuración y comandos](CONFIGURATION.md) y [compatibilidad de versiones](RELEASES.md). Los ajustes estrictos pueden romper el almacenaje incluso al dueño; un modpack completo necesita pruebas propias.

## Ownership / Titularidad

Copyright © 2026 Elgochogms. New 2.10.4 binaries: All Rights Reserved. Earlier releases retain their original license terms. This repository contains documentation and the original avatar only; no mod source, private maps, world data or secrets. Obfuscation raises the effort of inspecting Java bytecode but cannot make decompilation impossible.

