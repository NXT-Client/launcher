# NXT Resource Swapper

The NXT Resource Swapper lets the launcher and client replace Krunker assets
with local files before the game receives the original resource. It is intended
for textures, sounds, models, fonts, CSS, and similar static resources.

JavaScript files are intentionally not supported by the Resource Swapper.

## Folder Layout

The client creates the swapper directory inside the NXT user data folder:

```txt
%APPDATA%/NXT/NXTSwapper/
  README.txt
  resources/
  packs/
```

`resources/` is the loose-files area. Files placed here are treated as one pack
called `Loose Files`.

`packs/` contains separate resource packs:

```txt
%APPDATA%/NXT/NXTSwapper/
  resources/
    textures/weapons/weapon_1.png

  packs/
    Competitive Pack/
      pack.json
      textures/weapons/weapon_1.png
      sound/weapon_1.mp3

    Content Pack/
      pack.json
      textures/pubs/b_0.png
      models/example/model.obj
```

## Path Matching

Replacement files should use the same relative path as the Krunker asset.

Example:

```txt
Local file:
packs/Competitive Pack/textures/weapons/weapon_1.png

Can replace:
https://assets.krunker.io/textures/weapons/weapon_1.png
https://krunker.io/assets/textures/weapons/weapon_1.png
```

For `user-assets.krunker.io`, use a `user-assets/` prefix:

```txt
packs/My Pack/user-assets/61814/model.obj
```

## Pack Metadata

Each pack can include an optional `pack.json`:

```json
{
  "name": "Competitive Pack",
  "version": "1.0.0",
  "author": "NXT",
  "description": "Clean competitive replacements."
}
```

The launcher uses this metadata in the Pack Manager. If `pack.json` is missing,
the folder name is used as the pack name.

## Pack Manager

The launcher Resource Swapper tab shows all detected packs.

- Toggle a pack on or off.
- Move a pack up or down.
- Higher packs win conflicts.
- `Loose Files` is treated like a normal pack and can also be reordered.

After changing packs, use `Rescan`. If an already loaded map still shows old
assets, use `Clear Cache` and reload the map or restart the client.

## Conflict View

The Conflict View shows resources that are provided by more than one active
pack.

Example:

```txt
/textures/weapons/weapon_1.png
Using Competitive Pack; shadowing Content Pack
```

This means both packs contain the same target path, but `Competitive Pack` wins
because it has higher priority.

## Validation Report

The Validation Report shows files or folders the swapper could not safely use.

Common validation messages:

- unsupported file type
- file larger than 100 MB
- symlink skipped
- unsafe path skipped
- unreadable file or folder
- folder nested too deeply

Validation issues do not stop the whole swapper. The client skips only the
affected file or folder and keeps indexing valid resources.

## Supported File Types

The current supported extensions are:

```txt
.png
.jpg
.jpeg
.gif
.webp
.svg
.mp3
.ogg
.wav
.mp4
.webm
.obj
.mtl
.fbx
.glb
.gltf
.bin
.json
.css
.woff
.woff2
.ttf
.otf
```

## Safety Rules

The swapper deliberately avoids executable behavior.

- No JavaScript resources are accepted.
- Symlinks are skipped.
- Paths may not escape the pack folder.
- Files above 100 MB are skipped.
- Only local files inside `NXTSwapper` are served.
- The local asset server only accepts requests from the local machine.

## Recommended Workflow

1. Open the launcher.
2. Start the client so the launcher bridge is connected.
3. Open `Resource Swapper`.
4. Open the swapper folder.
5. Add files to `resources/` or create a pack in `packs/`.
6. Click `Rescan`.
7. Enable or reorder packs if needed.
8. Check `Conflict View` and `Validation Report`.
9. Clear cache or reload the map if old assets are still visible.
