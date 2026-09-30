# Silent Hill: Townfall - Internal Mod Menu | Full ESP, Puzzle Solver, Objective Guide

<p align="center">
  <img src="https://i.imgur.com/H5UZHCE.png" alt="Silent Hill Townfall Mod Menu" width="850"/>
</p>

<p align="center">
  <b>A comprehensive internal trainer and exploration tool for Silent Hill: Townfall.</b><br>
  Built with DirectX 12 hooks, native Unreal Engine 5 SDK integration, and bilingual localization (English / Kurdish).
</p>

<p align="center">
  <a href="#single-player-notice--disclaimer">Legal Notice</a> |
  <a href="#features">Features</a> |
  <a href="#screenshots">Screenshots</a> |
  <a href="#how-to-use--injection-instructions">How to Use</a> |
  <a href="#hotkeys">Hotkeys</a>
</p>

---

## Single-Player Notice & Legal Disclaimer

> **IMPORTANT NOTICE:**  
> * **Silent Hill: Townfall is strictly a single-player, offline story game.**  
> * This project does **NOT** provide any multiplayer advantages, bypass any online anti-cheat mechanisms, interact with online matchmaking, or affect any competitive multiplayer services.  
> * It is developed exclusively for offline single-player accessibility, puzzle-solving assistance, exploration, and reverse-engineering research.

#### DMCA / Copyright / Takedown Notice:
If you are a copyright holder, developer, or publisher of the game and have any concerns regarding this repository or any attached content, please contact me directly before filing any claims. I respect all intellectual property rights and will promptly comply with any formal removal requests:
- **Developer:** Ameer Xoshnaw
- **Contact:** Open an issue or discussion on this repository.

---

## Features

### Visuals & World ESP
- **Enemy ESP:** 2D bounding boxes (Full box or Corner box), dynamic health bars, distance display (meters), and real-time AI alert states (Calm, Investigating, Searching, Spotted, Stunned).
- **Passcode & Combination ESP:** Displays solutions for safe dials, lock boxes, and keypad combinations directly in the 3D world.
- **Door & Security ESP:** Marks open, unlocked, and locked doors along with the required keycard or physical key name.
- **Ground Item ESP:** Highlights dropped and spawned weapons, ammunition, medical items, and tools.
- **Objective & Quest Markers:** Distance markers and screen snaplines directly pinpointing your destination and required quest items.
- **Custom Screen Crosshair:** Cross, Circle, or Dot styles with customizable size and dynamic RGB rainbow animation.

---

### Puzzle Solver & HUD Navigation
- **Active Puzzle Solver HUD:** Automatically detects puzzles within 35 meters and calculates the correct solution on-screen (Combination Locks, BP_KeyPad_C digital keypads, Hospital Generator fuel valves, and X-Ray machine dials).
- **One-Click Auto Solve:** Solves and enters the correct solution directly without manual trial-and-error.
- **Progression & Chapter Walkthrough HUD:** Live on-screen guidance displaying:
  - Current Mission Name
  - Current Objective
  - What To Do (Step-by-step action hints)
  - Where To Go (Precise target locations)
  - Required story keys and items
- **Digital HP Counter HUD:** Floating numerical health readout anchored cleanly over the in-game health bar.

---

### Auto-Loot & 255+ Item Spawner
- **Universal Auto-Looter:** Press **V** to automatically open nearby closed containers, lockers, and health boxes, instantly collecting all loose ground items, ammo, and notes directly into your inventory.
- **Full Item Spawner:** Spawn any item into your inventory with custom quantity, ammo, durability, and skin variants:
  - Weapons & Ammunition
  - Medical Supplies: Gauze, Medkits, Syringes
  - Story Items: All Keys, Keycards, Cassette Tapes, and Floppy Disks
- **One-Click Bundles:** Essential Survival Kit, All Weapons + Max Ammo, and All Story Keys.

---

### Character, Camera & Movement
- **Third-Person Camera Mode:** Smooth shoulder-cam view with custom distance, side offset, and height sliders, while unhiding the full character body and clothes.
- **God Mode & Safe From Grapple:** Immunity from damage and instant-kill monster grabs.
- **Speedhack & Air Jump:** Multiplied running speed with infinite mid-air jumps.
- **Fly & NoClip:** Free flight mode to explore out-of-bounds areas and map architecture.
- **Passive Health Regen:** Configurable health recovery per second with hit-pause delay.
- **Character Switcher:** Play as Simon, Zoe, or Richard on any map.

---

### Combat & AI Exploits
- **Bullet Tracking (Magic Bullet):** Deflects fired rounds directly to chosen target bones (Head, Chest, Pelvis) without snapping your camera view.
- **Combat Aimbot:** Configurable FOV circle, smoothness slider, and aim key selector.
- **Infinite Ammo & Weapon Durability:** Never reload and weapons never degrade.
- **Rapid Fire & Instant Reload:** Removes pump-action delays and reload durations.
- **AI Freeze & Pacify:** Freeze enemy AI paths or reset alerted monsters back to a calm state.
- **Vacuum & Yeet:** Pull enemies together or launch them into the skybox.

---

### System & Localization
- **Instant Dual-Language Switch:** Seamless toggle between English and Kurdish (کوردی). Changes the ImGui menu, on-screen HUDs, and 3D world ESP markers in real time.
- **Save / Load Config:** Saves all preferences, toggles, colors, and hotkeys to TownfallModSettings.ini.

---

## Screenshots

| Menu Interface & Visuals | Progression Guide & World ESP |
|:---:|:---:|
| <img src="https://i.imgur.com/OCyHFIv.png" width="450"/> | <img src="https://i.imgur.com/6QXsoYp.png" width="450"/> |
| <img src="https://i.imgur.com/STo5pSu.png" width="450"/> | <img src="https://i.imgur.com/yarzEu1.png" width="450"/> |
| <img src="https://i.imgur.com/kbh1JRp.png" width="450"/> | <img src="https://i.imgur.com/8fSXyEx.png" width="450"/> |
| <img src="https://i.imgur.com/OsRmg0Y.png" width="450"/> | <img src="https://i.imgur.com/0vGvTXK.png" width="450"/> |
| <img src="https://i.imgur.com/2JUAfeq.png" width="450"/> | <img src="https://i.imgur.com/YjVbzsA.jpeg" width="450"/> |

---

## How to Use / Injection Instructions

> **IMPORTANT (TO PREVENT CRASHES):**  
> **Always inject while IN-GAME after loading your save file or level, NOT in the initial Main Menu or Lobby.**  
> *Injecting during the main menu or intro videos will cause an Access Violation crash because Unreal Engine's world viewport and player controller are not yet initialized.*

1. Launch **Silent Hill: Townfall** and load into the game world.
2. Open your preferred 64-bit DLL injector (such as **Process Hacker**, **Xenos**, or any standard injector).
3. Select the target process:  
   `Townfall-Win64-Shipping.exe`
4. Select the DLL file:  
   `SilentHillTownfall_ModMenu.dll`
5. Inject the DLL and return to the game window.

---

## Hotkeys

| Key | Action |
|:---:|:---|
| **INSERT** | Toggle Mod Menu GUI show / hide |
| **V** | Quick Universal Auto-Loot sweep (collects items and opens nearby containers) |
| **END** | Safely unhook and unload cheat DLL from the game process |

---

## Technical Details
- **Language:** C++20
- **Graphics API:** DirectX 12 (D3D12 Hooking)
- **GUI Library:** Dear ImGui
- **Hooking Framework:** MinHook
- **Target Architecture:** x64

---

## Credits
- **Ameer Xoshnaw** - Reverse engineering, SDK generation, feature implementation, and Kurdish localization.
- Unreal Engine modding and reversal community.
