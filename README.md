# DataPack-MDK
A Gradle project that can build Minecraft datapacks and export them in several formats.

## Current State
Currently this project can process and compile a datapack that will load as both a Forge and Fabric mod. 

## Setup
1. Edit `gradle.properties` to configure the name and version of your datapack.
2. Place your datapack files in `src/main/resources/data`
3. Run the `./gradlew build` command in the root project folder. This requires Java 16!
4. The JAR will be found in `./build/libs/`

The exported JAR will work in Forge or Fabric's mod folder. It will also work as a vanilla datapack.

## TODO
- Improve documentation
- Add project logo support
- Expose more properties to gradle.properties
- Move Forge/Fabric meta files to their own sourcesets?
- Document the project in greater detail.
- Explain how token replacement works.
- Add option for JSON minify
- Add option to export zip, only fabric, and only forge
- Add warnings and error detection
- Add option to convert existing datapacks into mods?
- Create example with CurseForgeGradle set up?