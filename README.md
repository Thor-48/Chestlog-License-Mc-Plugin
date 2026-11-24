# Chestlog

A lightweight moderation and anti-cheat utility plugin for Minecraft **1.21+** that monitors watched players when they open or close containers and automatically scans inventories for illegal or heavily modified items.

[![Modrinth](https://img.shields.io/badge/Modrinth-Download-00AF5C?style=for-the-badge&logo=modrinth&logoColor=white)](https://modrinth.com/plugin/chatblock-why_luca/)
[![Discord](https://img.shields.io/badge/Discord-Join%20Server-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.com/invite/D8DtJF2Jye)
[![Ko-fi](https://img.shields.io/badge/Ko--fi-Support-FF5E5B?style=for-the-badge&logo=ko-fi&logoColor=white)](https://ko-fi.com/why_luca)

---

## Features
* **Watchlist Monitoring:** Tracks only specific players added to the watchlist (`players.yml`) to keep server performance clean and logs focused.
* **Automatic Container Scanning:** Scans container inventories both when a watched player opens and closes them (chests, barrels, shulker boxes, hoppers, etc. – Ender Chests are excluded).
* **Illegal & Modified Item Detection:** Automatically flags suspicious items, including:
  * Enchantments exceeding vanilla max levels
  * Enchantments applied to unsupported items (e.g., enchanted bread)
  * Conflicting enchantments on the same item
  * Custom `PersistentDataContainer` tags, Custom Model Data, and Attribute Modifiers
* **Detailed JSONL Logging & Export:** Saves container access (`container-access.jsonl`) and flagged items (`suspicious-items.jsonl`) with exact coordinates, timestamps, and item NBT data, plus an easy one-command export into timestamped folders.

## Commands

| Command | Alias | Description | Permission |
| :--- | :--- | :--- | :--- |
| `/chestlog add <player>` | `/cl add <player>` | Add a player to the watchlist. | `chestlog.add` |
| `/chestlog remove <player>` | `/cl remove <player>` | Remove a player from the watchlist. | `chestlog.remove` |
| `/chestlog list` | `/cl list` | View all currently watched players. | `chestlog.list` |
| `/chestlog export` | `/cl export` | Export watchlist and logs into a timestamped folder. | `chestlog.export` |
| `/chestlog reload` | `/cl reload` | Reload the watchlist from `players.yml`. | `chestlog.reload` |
| `/chestlog status` | `/cl status` | View tracked player count, active sessions, and data path. | `chestlog.status` |

## Permissions

| Permission | Description | Default |
| :--- | :--- | :--- |
| `chestlog.add` | Allows adding players to the watchlist. | `op` |
| `chestlog.remove` | Allows removing players from the watchlist. | `op` |
| `chestlog.list` | Allows viewing the watchlist. | `op` |
| `chestlog.export` | Allows exporting Chestlog data. | `op` |
| `chestlog.reload` | Allows reloading the watchlist. | `op` |
| `chestlog.status` | Allows checking plugin status. | `op` |

## Installation
1. Download the latest `.jar` file from Modrinth.
2. Place the file into your server's `plugins` folder.
3. Restart or reload your server.

## Links & Support
* 🌐 **Website:** [why-luca.bot-keep.xyz](https://why-luca.bot-keep.xyz/)
* 💬 **Discord:** [Join the Discord Server](https://discord.com/invite/D8DtJF2Jye)
* ☕ **Support:** [Buy me a coffee on Ko-fi](https://ko-fi.com/why_luca)

## License
This project is licensed under the **Chestlog License** – see the [License file](https://github.com/Thor-48/Chestlog-License-Mc-Plugin/blob/main/License.md) for details.

*Copyright © 2026 Thor_48, Why_Luca, and Luca The Fox*
