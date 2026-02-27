# ⚔️ CURSED CLASH: Shadow Clan Rising

A browser-based 3D action game built with [Three.js](https://threejs.org/), inspired by Jujutsu Kaisen. Fight through endless waves of shadow clan ninjas as your favorite cursed energy wielder — no installation, no engine, just an HTML file and some FBX animations.

---

## 🎮 Playable Characters

### Satoru Gojo — *The Honored One*
Master of the Limitless cursed technique. Controls space itself with Infinity. Sword-based combat with long reach and Domain Expansion as his ultimate.

### Yuji Itadori — *Vessel of Sukuna*
Raw physical power amplified by cursed energy. Fast, relentless brawler with high damage, short range, and Black Flash as his ultimate.

---

## 🕹️ How to Play

| Action | PC | Mobile |
|---|---|---|
| Move | `WASD` / Arrow Keys | Left joystick |
| Sprint | Hold `Shift` | Sprint button (toggles) |
| Attack | Left Click | Attack button |
| Special Ability | `E` | Special button |
| Camera | Mouse drag | Drag right side of screen |
| Zoom | Scroll wheel | — |

**Survive as many waves as you can.** Each wave spawns more enemies that get faster, hit harder, and have more HP. Every 30 kills charges your special ability.

**10% chance** a giant ninja spawns — twice the size, triple the HP, three times the damage. Don't sleep on them.

**Passive healing** kicks in after standing still for 3 seconds, regenerating HP up to 75%. Complete a wave to fully heal.

**Mobile:** The game is playable horizontally only. Rotate your device if prompted.

---

## 🔧 Tech Stack

- **Three.js r152** — 3D rendering, scene management, shadows
- **FBXLoader** — character and enemy animations
- **SkeletonUtils** — skeletal mesh cloning for enemies
- **Pure HTML/JS** — no build step, no framework, no npm

Everything runs from a single `index.html`. Drop it in a folder with your FBX files, open it in a browser, and it works.

---

## 📁 Required FBX Files

Place these in the same directory as `index.html`:

**Gojo**
- `gojo_standing_Pose.fbx`
- `gojo_walking.fbx`
- `gojo_sprint.fbx`
- `attackgojo.fbx`
- `gojo_get_sword.fbx`

**Yuji**
- `yujistanding.fbx`
- `yujiwalk.fbx`
- `yujirun.fbx`
- `yujipunch.fbx`
- `yujientersthestage.fbx`

**Ninja Enemies**
- `ninja_standing.fbx`
- `ninja_walk.fbx`
- `ninja_run.fbx`
- `ninja_attack__made_it_as_goofy_as_possible_.fbx`

---

## 🚀 Running Locally

Because FBX files load via `fetch`, you need a local server — browsers block file:// requests for security.

**Option 1 — VS Code Live Server** (easiest)
Install the Live Server extension, right-click `index.html`, click *Open with Live Server*.

**Option 2 — Python**
```bash
python -m http.server 8000
```
Then open `http://localhost:8000`.

**Option 3 — Node**
```bash
npx serve .
```

---

## 🧩 Using This as a Base for Your Own Game

You're welcome to fork or clone this repository as a starting point for your own project, **under one condition:**

**You must credit the original creator in your README and in your game's UI.**

Credit must include:
- A visible mention of the original project: *CURSED CLASH by yuniorrguez13*
- A link back to this repository: `https://github.com/yuniorrguez13-a11y/shadow-clones`

### What you can do ✅
- Fork and build your own game on top of this codebase
- Add your own characters, maps, mechanics
- Use it for personal or educational projects
- Deploy your version publicly, as long as credit is visible

### What you cannot do ❌
- Remove or hide the original credit
- Claim you built the engine from scratch
- Resell or monetize it without explicit permission
- Submit it to game jams or competitions as fully original work without disclosure

> **If you publish a clone of this project without proper credit, the repository will be reported to GitHub for DMCA violation.** I actively check for forks and clones. Don't make it weird — just give credit, it takes 30 seconds.

---

## 🙏 Credits

- **Game & Code** — [yuniorrguez13](https://github.com/yuniorrguez13-a11y)
- **Three.js** — [threejs.org](https://threejs.org/)
- **Jujutsu Kaisen** — Original manga/anime by Gege Akutami / MAPPA. This is a fan project with no commercial intent.

---

## 📌 License

This project is released under a **custom non-commercial license**. You may use, modify, and distribute it for non-commercial purposes with attribution. Commercial use requires explicit written permission from the author.
