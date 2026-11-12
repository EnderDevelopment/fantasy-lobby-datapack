# Fantasy Lobby Datapack for Minecraft Java Edition

Fantasy Lobby Datapack is a Minecraft Java Edition datapack for version 1.21.4 that adds a custom void dimension and a fantasy lobby platform. It uses a load function, a Minecraft function load tag, a 100x100 quartz platform, and a central world spawn at coordinates 0, 65, 0.

## Install

1. Use Minecraft Java Edition 1.21.4.
2. Create or select a world.
3. Open the world save folder.
4. Open the `datapacks` directory.
5. Copy the project folder into `datapacks`, keeping `pack.mcmeta` and the `data` folder at the datapack root.
6. Enter the world and run:

```text
/reload
```

The load function is registered through Minecraft's function load tag and runs when the datapack loads.

## Use

The datapack includes the custom dimension `fantasy_lobby:void_world`.

To run the lobby setup in the current execution dimension, use:

```text
/function fantasy_lobby:load
```

The function creates a quartz platform from `(-50, 64, -50)` through `(49, 64, 49)`, producing a 100x100 block base. It then sets the world spawn to `(0, 65, 0)`.

To run the setup inside the custom void dimension, use:

```text
/execute in fantasy_lobby:void_world run function fantasy_lobby:load
```

To move a player to the center of that dimension, use:

```text
/execute in fantasy_lobby:void_world run tp @s 0 65 0
```

---

More Minecraft plugin projects by EnderDevelopment: https://github.com/EnderDevelopment

Project page: https://dash.enderdevelopment.com/community/0bd69c79-4204-4343-91f7-68726375a925?utm_source=github&utm_medium=readme&utm_campaign=auto_publish&utm_content=0bd69c79-4204-4343-91f7-68726375a925
