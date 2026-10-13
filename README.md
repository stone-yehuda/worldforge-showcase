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

The game's source is private while it's in development. This repo is the gallery, and the same
gallery is easier to browse as a page: **[stone-yehuda.github.io/worldforge-showcase](https://stone-yehuda.github.io/worldforge-showcase/)**.

**Contents:** [In the game](#in-the-game) · [The four factions](#the-four-factions) · [Building a base](#building-a-base) · [Armies and heroes](#armies-and-heroes) · [Field battles](#field-battles) · [Sieges](#sieges) · [Concept art](#concept-art) · [Under the hood](#under-the-hood)

---

## In the game

Three moments from ordinary play, with the interface on.

<table>
  <tr>
    <td colspan="2"><img src="assets/ingame_battle.jpg" alt="Two Concord armies collide" /><br /><sub><b>Battle lines.</b> Squads fight as formations, with shield walls, pikes and shock infantry.</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="assets/ingame_cavalry.jpg" alt="Dragoons charge a pike block" /><br /><sub><b>Counters.</b> Dragoons charge a pike block. A braced line breaks a cavalry charge.</sub></td>
    <td width="50%"><img src="assets/ingame_base_raid.jpg" alt="A Fervent warband raids a Concord base" /><br /><sub><b>Raid.</b> A Fervent warband hits a Concord town while its workers are still gathering.</sub></td>
  </tr>
</table>

## The four factions

**The Concord**: magic and machine in balance. Blue aether crystals in gold armatures, Gothic plate, and a senate of many houses and many races. *Order, ambition, and the throne that binds them.*
<img src="assets/concord_roster.jpg" alt="Concord units and hero" width="100%" />

**The Directive**: technology and discipline. Every soldier is issued the same kit, stamped from one die and marked with the brass gear-wheel. Pike blocks, shield lines, rifles and iron constructs.
<img src="assets/directive_roster.jpg" alt="Directive units and hero" width="100%" />

**The Fervent**: magic, volatile and proud. Their rune tattoos hold and channel their power, and their armor is partial because their skin carries the magic. *Emotion as weapon. Faith as armor.*
<img src="assets/fervent_roster.jpg" alt="Fervent units and hero" width="100%" />

**The Forewarned**: dark and experimental. Blackened iron, eagle-beast helms that hide every face, and a violet glow. *Outcasts who remember how the world almost ended.*
<img src="assets/forewarned_roster.jpg" alt="Forewarned units and hero" width="100%" />

## Building a base

A base grows through three stages over a match: an open settlement, a town behind a timber
palisade, and a capital ringed in stone. One row per faction.

<table>
  <tr>
    <th></th>
    <th width="31%">1. Settlement</th>
    <th width="31%">2. Palisade town</th>
    <th width="31%">3. Fortified capital</th>
  </tr>
  <tr>
    <td><b>Concord</b></td>
    <td><img src="assets/city_concord_stage1.jpg" alt="Concord settlement" /></td>
    <td><img src="assets/city_concord_stage2.jpg" alt="Concord palisade town" /></td>
    <td><img src="assets/city_concord_stage3.jpg" alt="Concord fortified capital" /></td>
  </tr>
  <tr>
    <td><b>Directive</b></td>
    <td><img src="assets/city_directive_stage1.jpg" alt="Directive settlement" /></td>
    <td><img src="assets/city_directive_stage2.jpg" alt="Directive palisade town" /></td>
    <td><img src="assets/city_directive_stage3.jpg" alt="Directive fortified capital" /></td>
  </tr>
  <tr>
    <td><b>Fervent</b></td>
    <td><img src="assets/city_fervent_stage1.jpg" alt="Fervent settlement" /></td>
    <td><img src="assets/city_fervent_stage2.jpg" alt="Fervent palisade town" /></td>
    <td><img src="assets/city_fervent_stage3.jpg" alt="Fervent fortified capital" /></td>
  </tr>
  <tr>
    <td><b>Forewarned</b></td>
    <td><img src="assets/city_forewarned_stage1.jpg" alt="Forewarned settlement" /></td>
    <td><img src="assets/city_forewarned_stage2.jpg" alt="Forewarned palisade town" /></td>
    <td><img src="assets/city_forewarned_stage3.jpg" alt="Forewarned fortified capital" /></td>
  </tr>
</table>

The same buildings and walls laid out side by side, from the in-game **Roster** viewer.

<img src="assets/roster_buildings.jpg" alt="Buildings of all four factions by tier" width="100%" />
<sub><b>Buildings by tier.</b> Concord · Directive (top), Fervent · Forewarned (bottom).</sub>

<img src="assets/roster_walls.jpg" alt="Wall sets of all four factions" width="100%" />
<sub><b>Walls.</b> Palisades in tier I, then stone ramparts, towers, stairs and gates in tier II.</sub>

## Armies and heroes

Rosters are built per faction, not shared and recoloured. Also from the Roster viewer.

<img src="assets/roster_armies.jpg" alt="Army rosters of all four factions" width="100%" />
<sub><b>Armies.</b> Each faction fills unit slots (spear, shield line, ranged, cavalry, siege and more) across three tiers, with a capstone unit.</sub>

<img src="assets/roster_heroes.jpg" alt="Hero halls and heroes of all four factions" width="100%" />
<sub><b>Heroes.</b> Each faction fields three commanders from its own hero hall.</sub>

## Field battles

Full armies on each of the four maps: infantry and constructs in the centre, ranged ranks and
siege engines behind. These scenes and the sieges below are staged in the engine with the
interface hidden.

<table>
  <tr>
    <td width="50%"><img src="assets/battle_brasswater_overview.jpg" alt="Concord and Directive armies on Brasswater Concourse" /><br /><sub><b>Brasswater Concourse.</b> Concord against Directive, beside the river.</sub></td>
    <td width="50%"><img src="assets/battle_heartwood_overview.jpg" alt="Concord and Fervent armies on Heartwood Wilds" /><br /><sub><b>Heartwood Wilds.</b> A Fervent warhost wraps around the Concord line.</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="assets/battle_ironroot_overview.jpg" alt="Directive and Forewarned armies on Ironroot Deeps" /><br /><sub><b>Ironroot Deeps.</b> Directive ranks curve around a Forewarned legion.</sub></td>
    <td width="50%"><img src="assets/battle_vigil_scar_overview.jpg" alt="Fervent and Forewarned armies on the Vigil Scar" /><br /><sub><b>The Vigil Scar.</b> Fervent warbands advance across the violet ash wastes.</sub></td>
  </tr>
</table>

<details>
<summary><b>Closer angles on the same four battles</b></summary>
<br />
<table>
  <tr>
    <td width="50%"><img src="assets/battle_brasswater_gunline.jpg" alt="View from behind the Directive line" /><br /><sub><b>Brasswater, behind the Directive line.</b> Cannon and ranged ranks behind the melee, the big constructs in the middle of it.</sub></td>
    <td width="50%"><img src="assets/battle_brasswater_cavalry_flank.jpg" alt="The battle seen from the flank" /><br /><sub><b>Brasswater, from the flank.</b> Siege engines drawn up behind the infantry.</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="assets/battle_heartwood_concord_ranks.jpg" alt="View from behind the Concord ranks" /><br /><sub><b>Heartwood, behind the Concord ranks.</b> Archers and siege engines in depth, looking toward the clash.</sub></td>
    <td width="50%"><img src="assets/battle_ironroot_melee_line.jpg" alt="View down the engaged line on Ironroot Deeps" /><br /><sub><b>Ironroot, down the line of contact.</b> The Directive's iron constructs in the thick of it.</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="assets/battle_vigil_scar_bombard_line.jpg" alt="Close view of the fight on the Vigil Scar" /><br /><sub><b>Vigil Scar, where the lines meet.</b> A Forewarned gun crew in the foreground, the Fervent line beyond.</sub></td>
    <td width="50%"></td>
  </tr>
</table>
</details>

## Sieges

Walls can be manned, gates can be held, and attackers bring siege towers to the rampart.

<table>
  <tr>
    <td width="50%"><img src="assets/siege_grand_assault_wide.jpg" alt="An army assaults a brick fortress" /><br /><sub><b>The assault.</b> Concord infantry and two siege towers close on a Directive fortress while its garrison lines the wall.</sub></td>
    <td width="50%"><img src="assets/siege_gate_clash_heroic.jpg" alt="Fighting at the fortress gate" /><br /><sub><b>At the gate.</b> A construct holds the gateway as the towers come up on either side.</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="assets/siege_rampart_overlook.jpg" alt="Defenders on the rampart walkway" /><br /><sub><b>On the wall.</b> The garrison on the walkway, with the stair up to it on the right.</sub></td>
    <td width="50%"><img src="assets/siege_obsidian_citadel.jpg" alt="A Fervent warband attacks a Forewarned citadel" /><br /><sub><b>The black citadel.</b> A Fervent warband storms Forewarned walls on the Vigil Scar.</sub></td>
  </tr>
</table>

## Concept art

<img src="assets/concept_art.jpg" alt="Worldforge concept art" width="100%" />

## Under the hood

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
