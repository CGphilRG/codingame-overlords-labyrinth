> 🇫🇷 [Version française](README_fr.md)

# Overlord's Labyrinth — CodinGame Multiplayer RPG SDK Project

A tactical RPG board duel inspired by **Wizardry IV: The Return of Nerdna** (summoning on Pentagrams) and **Conan Overlord** (Energy Gem allocation between summoning and double-activation), played on a **directional thin-wall labyrinth** (`0–F` hex bitmask `N=1, E=2, S=4, W=8` with edge-aware BFS) and featuring dynamic PixiJS switching between **2D RPG Sprites Mode** and **Geometric Debug Mode** (`ToggleModule`).

---

## Quick Commands
* **Local Web Viewer (`http://localhost:8888/test.html`)**:
  ```bash
  cd overlords-labyrinth-sdk
  mvn test-compile exec:java -Dexec.mainClass="Main" -Dexec.classpathScope="test"
  ```
* **Batch Simulation (3 Leagues)**:
  ```bash
  cd overlords-labyrinth-sdk
  mvn test-compile exec:java -Dexec.mainClass="Main" -Dexec.classpathScope="test" -Dexec.args="--simulate"
  ```
* **Switch CC0 Sprite Pack**:
  ```bash
  python3 scripts/apply_sprite_pack.py kenney-tiny-dungeon   # or kenney-roguelike-field / kenney-1bit-retro / legacy-dark-stone
  ```

---

## CodinGame & GitHub Links

* **CodinGame Contribution**: https://www.codingame.com/contribute/view/1586818a88014df499301a39a4dbd615c75dfe
* **Play in CodinGame IDE**: https://www.codingame.com/ide/demo/16057779640832b6c2b793a6dd8f1b789d4447d
* **GitHub Repository**: https://github.com/CGphilRG/codingame-overlords-labyrinth
* **6-Puzzle Showcase Hub (GitHub Pages)**: https://cgphilrg.github.io/codingame-sdk-puzzles/

> **Note:** League Boss files (`config/**/Boss.java`) are kept local-only and excluded via `.gitignore`.
