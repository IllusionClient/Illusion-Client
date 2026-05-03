# 🎮 Illusion Client

<div align="center">

![Java](https://img.shields.io/badge/Java-21+-orange?style=flat-square)
![Minecraft](https://img.shields.io/badge/Minecraft-1.21.11-brightgreen?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)
![Status](https://img.shields.io/badge/Status-Active-success?style=flat-square)

**A lightweight Minecraft 1.21.11 Fabric mod for PvP optimization**

</div>

---

## 📌 About

Illusion Client is a Minecraft 1.21.11 Fabric mod designed for PvP players who want performance optimizations and useful HUD features. Unlike heavy clients, Illusion focuses on minimal overhead while providing essential competitive features.

---

## 🚀 Quick Start

### Installation

1. **Download Fabric Loader** for Minecraft 1.21.11 from [fabricmc.net](https://fabricmc.net/use/)
2. **Download Fabric API** 0.141.1+ for 1.21.11
3. **Place this mod JAR** in your `.minecraft/mods/` folder
4. **Launch Minecraft** with Fabric profile

### First Launch
- Press **RIGHT SHIFT** in-game to open the settings menu
- Customize HUD positions by pressing **H** (drag elements with your mouse)
- Press **H** again to exit edit mode

---

## ✨ Features

### ⚡ Performance
- **FPS Boost Mode** - Disables clouds and entity shadows
- **Smooth FPS** - Caps at 60 FPS with VSync for stability
- **Fullbright** - Maximum gamma for dark areas
- **Entity Culling** - Optimizes entity rendering
- **Zoom** - Hold **C** for 70% FOV reduction

### 🎯 PvP HUD Modules
All HUD elements can be dragged to custom positions (press **H** to edit):

- **CPS Counter** - Shows clicks per second
- **Reach Display** - Shows attack reach distance
- **Combo Counter** - Tracks combo hits
- **Armor Durability** - Shows armor durability bars
- **Potion Timer** - Displays active potion effects
- **Key Strokes** - Shows WASD/Space/mouse button states
- **Sprint Toggle** - Visual indicator for sprint state
- **W-Tap Helper** - Shows when to W-tap for knockback
- **Attack Cooldown** - Visual bar for attack readiness
- **Target HUD** - Shows enemy health/distance when looking at them

### 🎨 Visual Customization
- **Purple Armor/Weapons** - All armor and weapons automatically tinted vibrant purple (Anglerfish-style)
- **Custom Hit FX** - Star-shaped particles spawn on hits (cyan for crits, purple for normal)
- **Hit Flash Effect** - Screen edge flash when taking damage
- **Modern Menu** - Dark UI with smooth toggle animations and scrolling

### 🔧 Utilities
- **Auto Sprint** - Automatically sprint when moving forward
- **HUD Edit Mode** - Press **H** to drag and reposition any HUD element
- **Scrollable Menu** - Mouse wheel to navigate long setting lists
- **Tabbed Interface** - "PvP & Visuals" and "Performance" tabs

---

## ⌨️ Keybinds

| Key | Action |
|-----|--------|
| **RIGHT SHIFT** | Open settings menu |
| **H** | Toggle HUD edit mode (drag elements) |
| **C** | Zoom (hold) |

---

## ⚙️ Configuration

Config file location:
```
Windows: %APPDATA%\.minecraft\illusion\config.json
```

### Available Settings

#### PvP & Visuals Tab
- Hitbox Visualiser - Show entity hitboxes
- Reach Display HUD - Show attack distance
- CPS Counter - Click speed display
- Sprint Toggle - Sprint state indicator
- Key Strokes HUD - Keyboard/mouse display
- Armour Durability HUD - Armor status
- Potion Timer HUD - Potion effect timers
- Hit Flash Effect - Damage screen flash
- Combo Counter - Combo tracker
- Custom Hit FX - Particle effects on hits
- W-Tap Helper - W-tap timing indicator
- Attack Cooldown HUD - Attack readiness bar
- Target HUD - Enemy info display
- Auto Sprint - Auto-sprint when moving

#### Performance Tab
- FPS Boost Mode - Disable clouds/shadows
- Entity Culling - Optimize entity rendering
- Particle Limiter - Reduce particles
- Chunk Anim Off - Disable chunk animations
- Smooth FPS - Cap at 60 with VSync
- FPS Counter HUD - Show FPS on screen
- Ping HUD - Show latency
- Fullbright - Max brightness
- Zoom Key (C) - Enable zoom

---

## 📁 Project Structure

```
Illusion-Client/
├── src/main/java/com/illusion/client/
│   ├── gui/
│   │   ├── IllusionMenuScreen.java    # Settings menu UI
│   │   ├── IllusionTitleScreen.java   # Custom title screen
│   │   └── HudEditScreen.java         # Transparent HUD edit overlay
│   ├── hud/
│   │   ├── HudRenderer.java           # Manages HUD rendering
│   │   └── HudModule.java             # Base class for HUD modules
│   ├── modules/
│   │   ├── pvp/                       # PvP modules
│   │   │   ├── ArmorCustomizationModule.java    # Purple armor
│   │   │   ├── WeaponCustomizationModule.java   # Purple weapons
│   │   │   ├── CustomHitEffectsModule.java      # Hit particles
│   │   │   ├── WTapHelperModule.java            # W-tap indicator
│   │   │   ├── AttackCooldownModule.java        # Attack bar
│   │   │   ├── TargetHudModule.java             # Enemy info
│   │   │   ├── AutoSprintModule.java            # Auto sprint
│   │   │   └── ... (other PvP modules)
│   │   └── performance/               # Performance modules
│   │       ├── FpsBoostModule.java
│   │       ├── ZoomModule.java
│   │       └── ...
│   ├── mixin/                         # Mixin injections
│   │   └── InGameHudMixin.java        # (disabled - vanilla crosshair)
│   └── config/
│       └── IllusionConfig.java        # Configuration storage
└── build.gradle                       # Gradle build config
```

---

## 🔧 Technical Details

### Built With
- **Fabric API** 0.141.1+ - Mod framework
- **Java 21** - Programming language
- **Mixin** - Code injection system

### Performance
- Minimal overhead (< 1ms per frame for UI)
- Armor/weapon color updates every 0.5 seconds (not every tick)
- Smart rendering - only updates when values change

---

## 📝 License

MIT License - See LICENSE file for details.

---

## ⚠️ Disclaimer

- This mod is for educational and personal use
- Some servers may prohibit modded clients - check server rules
- Not affiliated with Mojang/Microsoft
- Use at your own risk

---

<div align="center">

**Made for competitive Minecraft PvP**

[⬆ Back to top](#-illusion-client)

</div>
