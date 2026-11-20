# Dragon Block C - Galacticraft Space Flight (MC 1.7.10)

## Compilar
1. Descarga el **Forge MDK 1.7.10 (10.13.4.1614)** y copia de el a esta carpeta: `gradlew`, `gradlew.bat` y la carpeta `gradle/`
   (no se incluyen porque no se pudo descargar el wrapper). Usa JDK 8.
2. `gradlew setupDecompWorkspace`
3. `gradlew build`
4. El JAR queda en `build/libs/DBC-Galacticraft-SpaceFlight-1.7.10-1.0.0.jar`

## Instalar
Copia el JAR en `mods/` (cliente Y servidor) junto a Forge, Galacticraft Core/Planets y Dragon Block C. Se genera `config/dbcgcspace.cfg`.

## Config
entryHeight (2000), autoSpaceEntry, infiniteBreathing, hideOxygenUI, sourceDimension (0),
destinationDimension (-28 Luna), returnDimension (0), returnHeight (1950; -1 = sin regreso por descenso),
destinationEntryY (2050), returnSpawnY (1990), cooldownTicks (200), safeLanding.

## Notas
- Histeresis anti-bucle: entras a Y=2050 en destino; regresas a Y=1990 en Overworld (<2000). Cooldown extra por jugador.
- Con returnHeight activo, descender bajo esa Y en el destino te devuelve al Overworld; para aterrizar y explorar el planeta pon returnHeight=-1.
- Galacticraft se toca solo por reflexion/nombre de DamageSource: ningun JAR ajeno se modifica.
