
# ⚡ Pokémon Fighting Simulator

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,21,30&height=210&section=header&text=Pok%C3%A9mon%20Fighting%20Simulator&fontSize=46&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=Turn-Based%20Battles%2C%20Real%20Strategy&descAlignY=56&descSize=19" width="100%"/>

<br/>

[![Version](https://img.shields.io/badge/version-3.4.0-F7B801?style=for-the-badge&logo=pokemon&logoColor=black)](https://github.com)
[![Stack](https://img.shields.io/badge/React%20%7C%20TypeScript%20%7C%20Node-F18701?style=for-the-badge&logo=react&logoColor=white)](https://github.com)
[![License](https://img.shields.io/badge/license-MIT-F6AA00?style=for-the-badge&logo=opensourceinitiative&logoColor=black)](LICENSE)
[![Pokémon](https://img.shields.io/badge/pok%C3%A9mon-151-FFD60A?style=for-the-badge&logo=pokemon&logoColor=black)](https://pokemondb.net)

<br/>

### 🎮 A complete turn-based Pokémon battle simulator — with real type charts & mechanics

*⚔️ Gen 1–9 Types • 🧠 Smart AI • 📊 Stat Calculation • 🎨 Animated Battles*

<br/>

<a href="https://share.google/DnqnBzPuOthTipoY9">
  <img src="https://img.shields.io/badge/🎮_PLAY_NOW-F7B801?style=for-the-badge&logo=googlechrome&logoColor=black&labelColor=CC9700" alt="Play Now" height="45"/>
</a>
&nbsp;&nbsp;
<a href="https://share.google/DnqnBzPuOthTipoY9">
  <img src="https://img.shields.io/badge/📥_GET_SOURCE-F18701?style=for-the-badge&logo=github&logoColor=white&labelColor=C46D00" alt="Get Source" height="45"/>
</a>
&nbsp;&nbsp;
<a href="https://share.google/DnqnBzPuOthTipoY9">
  <img src="https://img.shields.io/badge/📚_DOCS-FFD60A?style=for-the-badge&logo=readthedocs&logoColor=black&labelColor=CCAB08" alt="Docs" height="45"/>
</a>

</div>

<img width="1280" height="720" alt="maxresdefault - 2026-11-10T224607 880" src="https://github.com/user-attachments/assets/bbcb3767-187c-4439-8237-0be7bdc52d11" />

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🌟 Overview

**Pokémon Fighting Simulator** is a **complete, playable turn-based battle engine** built in TypeScript. It implements real Pokémon mechanics — type effectiveness, stat calculation, damage formula, status conditions, and move priority — so every battle feels authentic.

Battle against a smart AI opponent or play hot-seat with a friend. The simulator covers the full battle flow: move selection, turn resolution, animations, HP tracking, and win/lose states.


<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🎯 Key Features

<div align="center">

| ⚔️ **Real Type Chart** | 📊 **Stat Calculation** | 🧠 **Battle AI** |
|:---:|:---:|:---:|
| Gen 1–9 type<br/>effectiveness | Base stats, IVs, EVs,<br/>natures & levels | Chooses best move<br/>based on matchup |

| 🎲 **Turn System** | 💫 **Status Effects** | 🎨 **Animated Battles** |
|:---:|:---:|:---:|
| Priority, speed ties,<br/>& switch logic | Burn, poison,<br/>paralysis & sleep | Move animations,<br/>HP bars & effects |

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🏆 Why This Simulator

<div align="center">

| 💎 **Advantage** | 📝 **Description** |
|:---|:---|
| 🧮 **Real Damage Formula** | Uses the official Gen 5+ damage formula — outputs match the real games |
| ⚔️ **Full Type Chart** | All 18 types with correct effectiveness, immunities & STAB |
| 🧠 **Competent AI** | Evaluates type matchup, HP, and switch options before acting |
| 🎨 **Beautiful Presentation** | Sprites, smooth animations, and clean battle UI |
| 📱 **Runs Everywhere** | Browser-based — works on desktop, tablet, and mobile |
| 🧩 **Mod-Friendly** | Add new Pokémon, moves, and abilities with JSON data files |

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🎬 Battle Preview

<div align="center">

```ascii
╔══════════════════════════════════════════════════╗
║  ⚡  Pokémon Fighting Simulator  v3.4.0          ║
╠══════════════════════════════════════════════════╣
║                                                  ║
║  👤 Your Team                     🤖 Opponent    ║
║  ──────────────────────────       ────────────   ║
║  ⚡ Pikachu  Lv.50                💧 Squirtle     ║
║  ❤️ 112/142                       ❤️ 98/130       ║
║                                                  ║
║  ⚔️ Turn 4                                       ║
║  ┌────────────────────────────────────────────┐  ║
║  │ ▶ Thunderbolt    ⚡ Electric    PP 15/15    │  ║
║  │   Quick Attack   ⚡ Normal      PP 30/30    │  ║
║  │   Iron Tail      ⚙️ Steel       PP 15/15    │  ║
║  │   Switch Pokémon                            │  ║
║  └────────────────────────────────────────────┘  ║
║                                                  ║
║  💥 Pikachu used Thunderbolt!                    ║
║     ⚡ Super effective! -68 HP                    ║
║                                                  ║
║  📊 Type: Electric vs Water = 2× damage          ║
╚══════════════════════════════════════════════════╝
```

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🧩 Project Structure

```
⚡ pokemon-fighting-simulator/
├── 🎯 src/
│   ├── engine/                # Battle engine
│   │   ├── damage.ts
│   │   ├── type-chart.ts
│   │   ├── stats.ts
│   │   └── status.ts
│   ├── ai/                    # Opponent logic
│   ├── ui/                    # Battle UI & animations
│   │   ├── battle-screen/
│   │   └── move-selector/
│   └── data/                  # Pokémon & move data
│       ├── pokemon.json
│       └── moves.json
├── 🎨 assets/                 # Sprites & sounds
├── 🧪 tests/                  # Damage & type tests
└── 📖 docs/                   # Mechanics reference
```

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🛠️ Tech Stack

<div align="center">

![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=for-the-badge&logo=vitest&logoColor=white)

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🤝 Community

Found a damage calc bug? Want to add a new Pokémon or move?

<div align="center">

<a href="https://share.google/DnqnBzPuOthTipoY9">
  <img src="https://img.shields.io/badge/💬_Join_Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" height="35"/>
</a>
<a href="https://share.google/DnqnBzPuOthTipoY9">
  <img src="https://img.shields.io/badge/🐞_Report_Issue-F7B801?style=for-the-badge&logo=github&logoColor=black" height="35"/>
</a>
<a href="https://share.google/DnqnBzPuOthTipoY9">
  <img src="https://img.shields.io/badge/⭐_Star_Repo-F18701?style=for-the-badge&logo=github&logoColor=white" height="35"/>
</a>

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 📜 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for details.

> ⚠️ **Copyright notice:** Pokémon, Pokémon character names, and related imagery are trademarks of **Nintendo, Creatures Inc., and GAME FREAK Inc.** This simulator is a **fan-made educational project** and is **not affiliated with or endorsed by** The Pokémon Company. No copyrighted assets are sold or redistributed commercially. Support the official games.

<br/>

<div align="center">

### ⚡ Made with 🎮 by the Pokémon Simulator Team

*If this simulator brought back memories — star the repo!*

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,21,30&height=120&section=footer" width="100%"/>

</div>
