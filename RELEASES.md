# ZoneProtes 2.9.1 — releases and compatibility

## English

- Pair: server 2.9.1 and client 2.9.1, one CurseForge project, split-1 handshake. Minecraft 1.20.1, Forge 47.x, Java 17.
- Required on the server: ZoneCore 2.1.3 or newer. This mod's client file does not require ZoneCore on the client.
- Changes from 2.9.0: new release metadata and ownership license, explicit server side ZoneCore dependency, protected distribution and rebuilt compatible client. Gameplay rules and wire protocol did not change.
- Optional integrations: ZoneClans, ZoneMap, ZoneEssentials, ZoneLevelUp, Create 6.0.8, Botania 456 and DivineRPG 1.10.7.5. The latter three were checked in earlier 2.9.0/2.8.x work, not in a full modpack with these protected files.
- Verification: both Gradle builds passed. The unprotected pair passed distribution checks and 273 isolated server fixture assertions with final ZoneCore 2.1.3 and ZoneCrates 2.0.6. The protected server started on Forge 47.4.10 with those mods, accepted /protes config estado and /protes reload, then stopped cleanly. A second startup with protected ZoneClans 1.1.4 logged its war integration as connected and shut down cleanly. Graphical client, two player network, other optional integrations with the protected JAR and production hosting remain untested here.
- Security: private implementation was obfuscated while preserving Forge entrypoint, JavaScript coremod hooks and public APIs required by other mods. The coremod script and public APIs remain inspectable. Never store secrets in a client JAR.
- Old MIT grants still apply to earlier MIT releases. The new 2.9.1 JAR declares All Rights Reserved.

## Español

- Pareja: servidor 2.9.1 y cliente 2.9.1 en un proyecto CurseForge, protocolo split-1. Minecraft 1.20.1, Forge 47.x, Java 17.
- Obligatorio en servidor: ZoneCore 2.1.3 o posterior. El cliente de este mod no requiere ZoneCore del lado cliente.
- Frente a 2.9.0: metadatos y licencia de la nueva entrega, dependencia ZoneCore indicada para servidor, distribución protegida y cliente compatible recompilado. Reglas de juego y protocolo sin cambios.
- Integraciones opcionales: ZoneClans, ZoneMap, ZoneEssentials, ZoneLevelUp, Create 6.0.8, Botania 456 y DivineRPG 1.10.7.5. Las tres últimas se comprobaron en trabajo anterior 2.9.0/2.8.x, no en un modpack completo con estos JAR protegidos.
- Verificación: compilaron ambos lados. La pareja sin proteger pasó separación y 273 comprobaciones en servidor aislado con ZoneCore 2.1.3 y ZoneCrates 2.0.6 finales. El servidor protegido arrancó en Forge 47.4.10 con esos mods, ejecutó /protes config estado y /protes reload, y cerró limpio. En otro arranque, ZoneClans 1.1.4 protegido declaró conectada su integración de guerras y el servidor cerró limpio. Aquí faltan cliente gráfico, dos jugadores, otras integraciones opcionales con JAR protegido y hosting.
- Seguridad: se ofuscaron partes internas conservando entrada Forge, ganchos JavaScript y APIs públicas necesarias para otros mods ZG. El script y las APIs públicas siguen siendo inspeccionables. No guardes secretos en el JAR cliente.
- Los permisos MIT de entregas anteriores siguen vigentes para ellas. El nuevo JAR 2.9.1 declara All Rights Reserved.

