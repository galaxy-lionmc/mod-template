## 🔧 Mod Info

* **Mod Name:** `Galatico Tier Tester`
* **Mod ID:** `galatico`
* **Author:** `galaxy_lionmc`
* **Package Name:** `com.galaxylion.galaticotiertester`
* **Minecraft Version:** `1.21`
* **Fabric Loader Version:** `0.19.1`
* **Yarn Mappings:** `1.21+build.9`
* **Fabric API Version:** `0.102.0+1.21`
* **Java Version (JDK):** `21`
* **Mod Type:** `client`

---

## 🧠 Mod Functionality

> A client-side PVP rank tracker mod. The mod tracks a player's performance in PVP through a point-based tier system. Points are gained and lost through combat events. The player must complete 20 games before their tier is revealed.
>
> **Point System:**
> - Hit a player → +15 points
> - Get hit by a player → -5 points
> - Lose a match (manual keybind G) → -20 points, counts as 1 completed game
> - Starting points: 0
>
> **Tier Ranges:**
> - HT1: 500–450 | LT1: 450–420
> - HT2: 420–400 | LT2: 400–350
> - HT3: 350–300 | LT3: 300–250
> - HT4: 250–200 | LT4: 200–150
> - HT5: 150–50  | LT5: 50–0
>
> **Tier Lock:** Player must complete 20 games before tier is calculated. During lock period the HUD shows "Tier: Locked" and a game counter (e.g. Games: 7/20). After 20 games, tier is assigned based on total points.
>
> **HUD (top-left corner):**
> - Updates every 5 seconds using a tick timer (no flicker, cached values)
> - Dark semi-transparent background behind text
> - During lock shows: [Galatico] / Mode: Sword | PVP / Games: 7/20 / Tier: Locked
> - After unlock shows: [Galatico] / Mode: Nethpot | SMP / Points: 312 / Tier: HT3
> - Tier text color: HT1=gold, HT2=yellow, HT3=green, HT4=aqua, HT5=gray (LT = dimmer versions of same)
>
> **Keybinds:**
> - H → opens Gamemode Select Screen
> - G → logs a match loss (-20 pts, +1 game, shows toast notification confirming it was logged)
>
> **Gamemode Select Screen (opens on H):**
> - Step 1: choose gamemode from 4 buttons in a grid: Sword, Nethpot, UHC, Axe & Shield
> - Step 2: choose type after picking gamemode: PVP (Player vs Player) or SMP (Many players)
> - Confirm button saves selection and closes the screen
> - Selected option is visually highlighted (green border or filled button)
> - Dark dimmed background overlay (standard Minecraft screen style)
> - Bottom of screen always shows: "Made by galaxy_lionmc — Support him on YouTube"
> - "Support him on YouTube" is a clickable underlined light-blue link that opens https://www.youtube.com/@Galaxy_LionMC in the browser using Util.getOperatingSystem().open(URI)
>
> **Data Persistence:**
> - Stats saved to: .minecraft/config/galatico/player_stats.json
> - Format: { "points": 312, "games_played": 22, "selected_mode": "Sword", "selected_type": "PVP" }
> - Loaded on game launch, saved on every stat change

---

## 📦 Output Instructions

The AI must:

* ✅ List all **Java source files**

  * Show full relative paths (e.g., `src/main/java/com/...`)
  * Give a one-line description of each file's purpose
* ✅ Write **full, working Java code** for every file

  * No placeholders, stubs, or missing logic
  * Fully import-ready and compilable
* ✅ Provide a valid, working `fabric.mod.json`
* ✅ Register all components correctly:

  * Items, blocks, screens, overlays, particles, keybinds, etc.
  * Client or server init logic as appropriate
* ✅ Include all required **import statements** and **annotations**

---

## 🎨 Assets (If Applicable)

If assets are needed, AI must:

* 📂 **List all required assets**, including:

  * Textures (`.png`)
  * Lang files (`lang/en_us.json`)
  * Models and blockstates (`.json`)
  * Sounds or GUI elements
* 📄 **Provide full content** and **exact paths** for each file:

  * Example: `src/main/.../exampleMixin.java`
  * Example: `src/main/resources/assets/[modid]/textures/item/example_item.png`
  * Example: `src/main/resources/assets/[modid]/lang/en_us.json`

---

## 📘 Documentation Output

Also generate a brief documentation file and save it as:

> 📁 `docs/OUTPUT.md`

This file must:

* ✅ Explain what the mod does
* ✅ Summarize all the components (classes, assets, events)
* ✅ Describe where everything is registered and how it works
* ✅ Be written for the user to understand how the mod is structured
* ✅ Use Markdown formatting (headings, bullets, code blocks)

---

## ⚙️ Optional Features

If applicable, include:

* Mixin setup
* Config file support (Cloth Config or JSON)
* Command registration
* Client/server networking
* Runtime environment checks
* Shader or render layer support

---

## ❌ Rules

* ❌ Do not skip any code
* ❌ Do not use vague notes like "implement this later"
* ❌ Do not generate placeholder files or comments
* ✅ Output must be **complete and build-ready** from the start