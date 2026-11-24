> 🇬🇧 [English version](README.md)

# Overlord's Labyrinth — Projet CodinGame Multiplayer RPG SDK

Un puzzle multijoueur RPG tactique inspiré de **Wizardry IV: The Return of Nerdna** (invocation sur pentagrammes) et **Conan Overlord** (allocation de gemmes d'énergie entre invocation et double activation), sur un **labyrinthe à cloisons fines directionnelles** (masque hexadécimal `0–F` : `N=1, E=2, S=4, O=8` avec BFS sur arêtes) et avec bascule dynamique PixiJS entre **Mode Sprites RPG 2D** et **Mode Formes Géométriques Debug** (`ToggleModule`).

---

## Commandes Rapides
* **Viewer Web Local (`http://localhost:8888/test.html`)** :
  ```bash
  cd overlords-labyrinth-sdk
  mvn test-compile exec:java -Dexec.mainClass="Main" -Dexec.classpathScope="test"
  ```
* **Simulation Batch (3 ligues)** :
  ```bash
  cd overlords-labyrinth-sdk
  mvn test-compile exec:java -Dexec.mainClass="Main" -Dexec.classpathScope="test" -Dexec.args="--simulate"
  ```
* **Changer de banque de sprites CC0** :
  ```bash
  python3 scripts/apply_sprite_pack.py kenney-tiny-dungeon   # ou kenney-roguelike-field / kenney-1bit-retro / legacy-dark-stone
  ```

---

## Liens CodinGame & GitHub

* **Contribution CodinGame** : https://www.codingame.com/contribute/view/1586818a88014df499301a39a4dbd615c75dfe
* **Jouer dans l'IDE CodinGame** : https://www.codingame.com/ide/demo/16057779640832b6c2b793a6dd8f1b789d4447d
* **Dépôt GitHub** : https://github.com/CGphilRG/codingame-overlords-labyrinth
* **Portail GitHub Pages (6 Puzzles)** : https://cgphilrg.github.io/codingame-sdk-puzzles/

> **Note :** Les fichiers Boss par ligue (`config/**/Boss.java`) sont conservés en local uniquement et exclus via `.gitignore`.
