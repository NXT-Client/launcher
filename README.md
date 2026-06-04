<a id="readme-top"></a>

![GitHub Tag](https://img.shields.io/github/v/tag/vaqqq/NXT-client?style=for-the-badge&label=version)
![License](https://img.shields.io/badge/Proprietary-green?style=for-the-badge&label=License)
![Launcher](https://img.shields.io/badge/NXT-Launcher-7C4DFF?style=for-the-badge)
![Windows](https://img.shields.io/badge/Windows-x64-0078D4?style=for-the-badge&logo=windows)
![Discord](https://img.shields.io/discord/1269411543615930421?style=for-the-badge&label=Discord&color=%237289da&link=https%3A%2F%2Fdiscord.gg%2FmE6KyEeVMK)

<br />
<div align="center">
  <a href="https://github.com/vaqqq/nxt-client">
    <img src="https://raw.githubusercontent.com/vaqqq/nxt-client/main/src/assets/logo-dark.png" alt="NXT Client Logo" width="360">
  </a>

  <h3 align="center">NXT Launcher</h3>

  <p align="center">
    The central place to install, update, customize, and manage the NXT Client.
    <br />
    <a href="#getting-started"><strong>Getting Started &raquo;</strong></a>
    <br />
    <br />
    <a href="https://discord.gg/mE6KyEeVMK">Report Bug</a>
    &middot;
    <a href="https://discord.gg/mE6KyEeVMK">Request Feature</a>
  </p>
</div>

---

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-launcher">About the Launcher</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#installation">Installation</a></li>
        <li><a href="#client-bridge">Client Bridge</a></li>
      </ul>
    </li>
    <li>
      <a href="#features">Features</a>
      <ul>
        <li><a href="#dashboard">Dashboard</a></li>
        <li><a href="#install-update-and-repair">Install, Update, and Repair</a></li>
        <li><a href="#mods">Mods</a></li>
        <li><a href="#crosshair-editor">Crosshair Editor</a></li>
        <li><a href="#matchmaker">Matchmaker</a></li>
        <li><a href="#resource-swapper">Resource Swapper</a></li>
        <li><a href="#userscripts">UserScripts</a></li>
        <li><a href="#quick-editor">Quick Editor</a></li>
        <li><a href="#logs-and-diagnose">Logs and Diagnose</a></li>
      </ul>
    </li>
    <li><a href="#verification">Verification</a></li>
    <li><a href="#notes">Notes</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

---

<!-- ABOUT THE LAUNCHER -->
## About the Launcher

<a href="https://github.com/vaqqq/nxt-client">
  <img src="https://raw.githubusercontent.com/vaqqq/nxt-client/main/src/assets/icon.ico" alt="NXT Icon" width="60" height="60">
</a>

Welcome to the NXT Launcher.

The launcher is built to make the NXT Client easier to use from the moment you
install it. Instead of manually downloading builds, checking versions, opening
folders, or changing client files yourself, the launcher gives you one clean
interface for the most important client tools.

It is not only a play button. It is a hub for updates, customization, resource
packs, scripts, diagnostics, and live Krunker information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

<!-- GETTING STARTED -->
## Getting Started

### Installation

1. Download the latest NXT Launcher release.
2. Start `NXT Launcher.exe`.
3. If the client is not installed yet, the launcher will offer to install it.
4. After installation, use the main button to start NXT.

The launcher can show download progress, installation progress, and the current
client status directly in the sidebar.

### Client Bridge

Some launcher tools need the NXT Client to be running.

When the client is open, the launcher connects through the local Client Bridge.
Once connected, features such as Mods, Resource Swapper, Matchmaker, UserScripts,
Quick Editor, and Diagnostics can sync directly with the client.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

<!-- FEATURES -->
## Features

### Dashboard

![Dashboard](https://img.shields.io/badge/Dashboard-383838?style=for-the-badge)

The Dashboard gives you a quick overview of NXT and Krunker.

- Start, install, update, or repair the client from one button.
- See the installed client version.
- Check whether the Client Bridge is connected.
- Check whether the Client Update Server is reachable.
- Open the client folder.
- Join the NXT Discord.
- See live Krunker player count and active matches.
- See Krunker status.
- View latest Krunker videos.
- View news, events, and live top maps.

---

### Install, Update, and Repair

![Updates](https://img.shields.io/badge/Updates-383838?style=for-the-badge)
![Repair](https://img.shields.io/badge/Repair-383838?style=for-the-badge)

The launcher can manage the client without users having to manually replace
files.

- Install the client when no installation is found.
- Detect available client updates.
- Detect launcher updates.
- Download updates through the launcher.
- Clear client cache.
- Restart the client.
- Open the client folder.

The launcher button changes depending on the current state:

| State | Meaning |
|-------|---------|
| `Install` | The client is missing and can be installed. |
| `Update` | A newer client version is available. |
| `Play` | The client is ready to start. |
| `Running` | The client is already open. |
| `Repair` | The local runtime or install state needs attention. |

---

### Mods

![Sky Color](https://img.shields.io/badge/Sky%20Color-383838?style=for-the-badge)
![CSS](https://img.shields.io/badge/CSS-383838?style=for-the-badge)
![Visuals](https://img.shields.io/badge/Visuals-383838?style=for-the-badge)

The Mods tab is made for visual customization and client-side resource options.

#### Sky Color

Change the look of the in-game sky directly from the launcher.

- Enable or disable custom sky colors.
- Pick a color manually.
- Use preset colors.
- Override dome gradient colors.
- Override fog color and fog distance.
- Override ambient color and intensity.
- Override light color and intensity.

#### Map Visuals

Adjust small visual parts of the game.

- Hide cats.
- Hide clouds.
- Replace billboard textures.
- Use an image URL.
- Upload a local image.
- Use the NXT logo as billboard replacement.

#### CSS

Manage client CSS modes without searching through folders.

- `Custom`: use selected custom CSS files.
- `Swapper`: use CSS from the swapper folder.
- `Client`: use built-in NXT CSS themes.
- `Disabled`: turn client CSS off.

You can upload separate CSS files for in-game and social pages.

---

### Crosshair Editor

![Crosshair](https://img.shields.io/badge/Crosshair%20Editor-383838?style=for-the-badge)

The Crosshair Editor lets you create, preview, import, export, and manage custom
crosshairs from the launcher.

- Enable or disable the custom crosshair.
- Hide the native Krunker crosshair.
- Create new crosshairs.
- Duplicate, rename, and delete crosshairs.
- Import and export crosshair JSON.
- Export a crosshair as PNG.
- Copy and import crosshair codes.
- Use separate Hip Fire and ADS variants.
- Copy Hip Fire settings to ADS or ADS settings to Hip Fire.
- Preview crosshairs on different backgrounds.
- Enable a pixel grid for detailed editing.
- Use class bindings for primary, secondary, and melee setups.

The editor supports shape, color, image, effects, transform, and utility
controls.

---

### Matchmaker

![Matchmaker](https://img.shields.io/badge/Matchmaker-383838?style=for-the-badge)

The Matchmaker tab helps you find better public matches faster.

- Load public matches from the Krunker matchmaker.
- Filter by region.
- Filter by game mode.
- Filter by map.
- Set minimum player count.
- Set minimum time left.
- Limit result count.
- Sort by most players, most time left, least time left, or almost full.
- Refresh manually or use auto-refresh.
- Apply your filters to the client.

The Quick Match Hook can use your launcher filters when pressing Krunker's Quick
Match button. If no filtered game is available, it can fall back to native Quick
Match.

---

### Resource Swapper

![Resource Swapper](https://img.shields.io/badge/Resource%20Swapper-7C4DFF?style=for-the-badge)
![Packs](https://img.shields.io/badge/Pack%20Manager-383838?style=for-the-badge)
![Priority](https://img.shields.io/badge/Priority-383838?style=for-the-badge)

The NXT Resource Swapper is our own pack-based resource system for the client.

Instead of only dropping files into one folder, the launcher lets you manage
resources as packs.

- Enable or disable the Resource Swapper.
- Open the swapper folder.
- Rescan resources.
- Clear cached resources.
- See detected file count, total size, and last scan time.
- Manage multiple resource packs.
- Enable or disable individual packs.
- Change pack priority.
- Use loose files as a pack.
- See which pack wins when multiple packs replace the same resource.
- View conflicts before they become confusing in-game.
- View validation reports for unsupported files, unsafe paths, large files, or
  unreadable resources.

Higher-priority packs win conflicts. This makes it easier to combine multiple
packs without manually moving files around.

For more details, see [`resource-swapper.md`](./resource-swapper.md).

---

### UserScripts

![UserScripts](https://img.shields.io/badge/UserScripts-383838?style=for-the-badge)
![Safe Mode](https://img.shields.io/badge/Safe%20Mode-383838?style=for-the-badge)

UserScripts can be managed directly from the launcher.

- Enable or disable UserScripts globally.
- Enable Safe Mode.
- Import local `.js` files.
- Import scripts from a URL.
- Install NXT Team Scripts.
- Enable or disable individual scripts.
- Edit script name, version, author, category, and run timing.
- Choose permissions such as DOM, CSS, Storage, and Network.
- Edit script content.
- Save changes.
- Run a script manually.
- Temporarily disable a script.
- Delete scripts.
- View script warnings and console output.

Safe Mode is useful when a script causes issues and you want to start the client
without running custom scripts.

---

### Quick Editor

![Quick Editor](https://img.shields.io/badge/Quick%20Editor-383838?style=for-the-badge)

The Quick Editor is a launcher-side tool for adjusting selected in-game UI
elements.

- Scan the current client DOM.
- Select detected UI elements.
- Move elements on a visual canvas.
- Set X and Y position.
- Choose anchors such as center, top left, top right, bottom left, and bottom
  right.
- Apply layout changes to the client.
- Reset custom layout changes.

This is intended to make UI positioning easier without editing scripts or CSS
manually.

---

### Logs and Diagnose

![Diagnostics](https://img.shields.io/badge/Logs%20%26%20Diagnose-383838?style=for-the-badge)

The Logs and Diagnose tab helps with support and troubleshooting.

- View client version and platform.
- View process ID and uptime.
- View memory usage.
- View the client user data path.
- Refresh diagnostic data.
- Copy diagnostics.
- Open the logs folder.
- Read recent client logs inside the launcher.

If something does not work correctly, this tab should make it easier to collect
the information needed for support.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

<!-- VERIFICATION -->
## Verification

![Verified](https://img.shields.io/badge/Verified%20Client-58D68D?style=for-the-badge)

The launcher can check whether the installed client matches the trusted release
information.

This helps users see whether their installed client is the expected NXT build.
It is shown as a small verification badge next to the main action button.

Security is not the main purpose of the launcher, but verification helps make
updates and installations more transparent.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

<!-- NOTES -->
## Notes

- Some features require the NXT Client to be running.
- Some features require the Client Bridge to be connected.
- Live Krunker data depends on public Krunker services.
- Resource Swapper and UserScripts are local customization features.
- The launcher is designed to make common client tasks easier, cleaner, and
  faster.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

<!-- CONTACT -->
## Contact

- Discord Support Server - [[Click Here]](https://discord.gg/mE6KyEeVMK)
- Website - [nxt-client.com](https://nxt-client.com/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---
