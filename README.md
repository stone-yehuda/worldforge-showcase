<p align="center">
  <img src="assets/banner.jpg" alt="Worldforge — a science-fantasy RTS" width="100%" />
</p>

<p align="center">
  <img alt="Godot 4" src="https://img.shields.io/badge/Godot_4.7-478CBF?style=flat-square&logo=godotengine&logoColor=white" />
  <img alt="GDScript" src="https://img.shields.io/badge/GDScript-355570?style=flat-square" />
  <img alt="Forward+" src="https://img.shields.io/badge/Renderer-Forward%2B-1c1917?style=flat-square" />
  <img alt="Status" src="https://img.shields.io/badge/Status-In_active_development-d4a017?style=flat-square" />
</p>

**Worldforge** is an original real-time strategy game I'm building in Godot 4, set in a world where
magic and technology amplify each other. Enchantment makes engines burn hotter; runes let bullets
punch through armor. Four societies each built themselves around one answer to how far that
should go, and the uneasy peace between them is cracking.

The game's source is private while it's in development. This repo is the gallery.

---

## ⚔️ In the game

<table>
  <tr>
    <td width="50%"><img src="assets/ingame_battle.jpg" alt="Two Concord armies collide" /><br /><sub><b>Battle lines.</b> Squads fight as formations, with shield walls, pikes and shock infantry.</sub></td>
    <td width="50%"><img src="assets/ingame_base_raid.jpg" alt="A Fervent warband raids a Concord base" /><br /><sub><b>Raid.</b> A Fervent warband hits a Concord town while its workers are still gathering.</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="assets/ingame_cavalry.jpg" alt="Dragoons charge a pike block" /><br /><sub><b>Counters.</b> Dragoons charge a pike block. A braced line breaks a cavalry charge.</sub></td>
    <td width="50%"><img src="assets/roster_heroes.jpg" alt="Hero halls and heroes of all four factions" /><br /><sub><b>Heroes.</b> Each faction fields three commanders from its own hero hall.</sub></td>
  </tr>
</table>

## 🏰 Bases, armies & walls

Every faction has its own architecture, tiered roster and fortifications. These shots come from
the in-game **Roster** viewer.

<img src="assets/roster_buildings.jpg" alt="Buildings of all four factions by tier" width="100%" />
<sub>Buildings by tier: Concord · Directive (top), Fervent · Forewarned (bottom).</sub>

<img src="assets/roster_armies.jpg" alt="Army rosters of all four factions" width="100%" />
<sub>Armies: each faction fills unit slots (spear, shield line, ranged, cavalry, siege and more) across three tiers, with a capstone unit.</sub>

<img src="assets/roster_walls.jpg" alt="Wall sets of all four factions" width="100%" />
<sub>Walls: palisades in tier I, then stone ramparts, towers and gates in tier II.</sub>

## 🛡️ The four factions

**The Concord**: magic and machine in balance. Blue aether crystals in gold armatures, Gothic plate, and a senate of many houses and many races. *Order, ambition, and the throne that binds them.*
<img src="assets/concord_roster.jpg" alt="Concord unit portraits" width="100%" />

**The Directive**: technology and discipline. Every soldier is issued the same kit, stamped from one die and marked with the brass gear-wheel. Pike blocks, shield lines, rifles and iron constructs.
<img src="assets/directive_roster.jpg" alt="Directive unit portraits" width="100%" />

**The Fervent**: magic, volatile and proud. Their rune tattoos hold and channel their power, and their armor is partial because their skin carries the magic. *Emotion as weapon. Faith as armor.*
<img src="assets/fervent_roster.jpg" alt="Fervent unit portraits" width="100%" />

**The Forewarned**: dark and experimental. Blackened iron, eagle-beast helms that hide every face, and a violet glow. *Outcasts who remember how the world almost ended.*
<img src="assets/forewarned_roster.jpg" alt="Forewarned unit portraits" width="100%" />

## 🖼️ Concept art

<img src="assets/concept_art.jpg" alt="Worldforge concept art" width="100%" />

## 🔧 What's under the hood

- **Asymmetric factions.** Rosters are defined per faction, so each slot means something different
  for each side, and some factions deliberately leave a slot empty.
- **Squad combat.** Units fight in formations. An armor and ward damage model, knockback, braced
  pikes and charge impacts run on a fixed 30 Hz simulation.
- **Enemy AI** runs its own economy, builds a base and sends attack waves.
- **Headless match simulator** plays whole AI-vs-AI matches without a renderer, for balance
  sweeps across seeds.
- **Heroes, tech trees and siege** sit on top of a Tech / Magic / Fusion research system.
- **Built with a multi-agent workflow.** Claude Code, Codex and Gemini work on one repo under
  shared rules for claiming tasks, reviewing each other's work and running worktrees.

## Credits

Concept art and unit portraits were generated locally with FLUX.1, then reviewed, curated and edited. Only approved pieces appear here.
In-game 3D models are partly original and partly adapted from CC0 packs by
[Kenney](https://kenney.nl), [KayKit](https://kaylousberg.itch.io) and
[Quaternius](https://quaternius.com).

<sub>© Yehuda Stone. All rights reserved. Images are shared here for portfolio viewing only.</sub>
