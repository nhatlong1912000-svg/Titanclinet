# TitanClient (starter source)

This is a **starter Fabric client mod project**, not a finished hacked client and not a built JAR.

## Important version note
The starter is configured for **Minecraft 1.21.11** because its dependencies are pinned to a known compatible baseline. It is **not configured for 1.21.111**. Do not install it as if it were a 1.21.111 mod. Update Minecraft, Yarn mappings, Fabric Loader, Fabric API, and the `fabric.mod.json` constraint together before targeting another version.

## Included
- TitanClient client entrypoint
- module registry with categories
- placeholder module entries for `Sus Chunk V2` and `Chunk Finder Prime`
- Right Shift keybind that currently prints module status

## Build
Install JDK 21 and Gradle, open this folder in a Java IDE, then run:

```bash
gradle build
```

The output JAR will be under `build/libs/` if the build succeeds.

## Current limitations
The menu screen, highlight rendering, waypoint storage/rendering, and chunk/base detection are not implemented yet. A normal client cannot reliably identify every hidden player base from ordinary chunk data alone. Add detection only for observable, legitimate signals and test in a world/server where such tools are allowed.


Build verification note: this source was updated for Minecraft 1.21.11, but the build was not verified in the current environment because Gradle and the required remote dependencies are unavailable here. The module registry is a scaffold; the named base-finding modules do not yet implement actual base detection.
