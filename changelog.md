# Changelog
All notable changes to this Minecraft 1.21.11 PvP/Optimization client will be documented here.  
This project follows Semantic Versioning: **MAJOR.MINOR.PATCH**

# 1.0.1
# ⚡ Performance Improvements
Added FPS Boost mode toggle (disables entity shadows & clouds)
Added Smooth FPS option for frame pacing
Added Entity Culling toggle for render optimization
# 🎯 Input & Responsiveness
(No changes in this version)
# 🖥️ Rendering & Visual Optimization
Added Fullbright toggle for maximum brightness
Added Hit Flash effect toggle
Added Custom Hit FX toggle
# 🧠 Engine / System Tweaks
Refactored module registration system to separate HUD-visible vs background-only modules
Auto-sprint now runs as background feature (no HUD positioning needed)
# 🎨 UI / UX
Complete Title Screen redesign: Scrolling starfield background, parallax effect, modern white button styling with colored accent bars
Complete Menu Screen redesign (Right Shift):
New 440×320 panel layout with sidebar tabs
Three organized categories: ⚔ COMBAT, 🎨 VISUALS, ⚡ ENGINE
Smooth animated toggles with lerp transitions
Clean dark theme with purple accent colors
Removed problematic scale animations (API compatibility)
Standardized button sizing (200×28) and spacing
Updated footer text styling with fade-in animations
# 🌐 Networking / Ping Stability
(No changes in this version)
# 🛠 Bug Fixes
Fixed config field name references (case sensitivity: fullbright, smoothFPS, fpsBoostMode)
Fixed clearAndInitWidgets() compatibility issue (changed to clearChildren())
Fixed MatrixStack.scale() API incompatibility by removing transform operations
# 🧹 Removed / Deprecated
HUD Changer (H key): Removed non-positionable modules from drag-drop editor:
Armor Customization (auto-enabled background feature)
Weapon Customization (auto-enabled background feature)
Auto-sprint (always-on utility)
Removed unused palette constants (C_GLASS, C_BTN_BASE, C_BTN_OUTLINE, etc.)
Removed grid background effect from title screen (simplified to stars only)
Removed chromatic glitch logo effect
