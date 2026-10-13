# SpaceSidePews

A free, retro-flavored side-scrolling shooter with modern neon graphics, a blend of a classic "fly the whole looping world" arcade shooter and a classic power-up-meter shooter. Hunt down organic hives in a wide looping world, fight through forced-scroll corridors, and beat a boss at the end of every stage.

**Play it in your browser:** https://nbwillcox.github.io/SpaceSidePews/

Everything is generated in code: sprites are vector-drawn on the fly, and all sound effects and music are synthesized with the Web Audio API. There are no image or audio files and no build step. A sibling of [SpaceGalaShooter](https://github.com/nbwillcox/SpaceGalaShooter), [SpaceCentiShooter](https://github.com/nbwillcox/SpaceCentiShooter), [SpaceVaderShooter](https://github.com/nbwillcox/SpaceVaderShooter), [SpaceStroids](https://github.com/nbwillcox/SpaceStroids), [SpaceCommand](https://github.com/nbwillcox/SpaceCommand), [lightCycles](https://github.com/nbwillcox/lightCycles), [SpaceRoboShooter](https://github.com/nbwillcox/SpaceRoboShooter) and [SpaceBricks](https://github.com/nbwillcox/SpaceBricks), with the same look and feel.

## Controls

| Action | Keys |
| --- | --- |
| Fly (8 directions) | `W` `A` `S` `D` or the arrow keys |
| Fire (hold to auto-fire) | `Space` or left mouse button |
| Reverse facing (free-flight stages) | `Shift` |
| Cash in the highlighted power-up | `E` or `Enter` |
| Smart bomb | `B` or right mouse button |
| Hyperspace (free-flight stages) | `H` |
| Pause | `P` or `Esc` |

### On a phone or tablet

Play in landscape. A floating stick on the left flies the ship; on the right, **FIRE** (hold), **REV** reverses, **POWER** cashes in the power-up meter, **BOMB** and **HYPER**. The pause button opens the menu. The on-screen controls appear on touch devices automatically; Settings has size, opacity and a left-handed layout. Use your browser's *Add to Home Screen* to install it as a full-screen app.

## Gameplay

- Stages alternate between two styles:
  - **Free-flight stages** (1, 3, 5...) take place in a wide looping world with a radar strip across the top. Destroy every **hive** (they spawn larvae and fire spore bursts) to open the gate to the boss. Reverse your facing with `Shift` to shoot enemies behind you.
  - **Forced-scroll stages** (2, 4, 6...) scroll upward through an organic corridor with scripted waves, wall turrets and tentacles. The walls are deadly. Reach the end to meet the boss.
- **Power-up meter:** wipe out a whole formation to drop a power capsule. Each capsule advances the highlight along the bottom meter (SPEED, MISSILE, DOUBLE, LASER, OPTION, SHIELD); press `E` to cash in the highlighted slot. Options are glowing orbs that trail your ship and copy your fire.
- Any hit is fatal and costs you every power-up except SPEED, but you respawn on the spot with a few seconds of invulnerability. A shield absorbs three hits.
- **Smart bombs** clear the screen (and chip hives and bosses). **Hyperspace** teleports you somewhere else in the world, with a small risk of a bad jump.
- Bosses (The Watcher, Overmind and Mother Core) have guard parts you must break before the core is exposed.
- Five organic themes and an endless stage count with rising difficulty. Local top-10 high scores with arcade-style 3-letter initials (stored in your browser).

## Run locally

It is plain HTML/CSS/JS. Either open `index.html` directly, or serve the folder:

```bash
python -m http.server 8000
```

then visit http://localhost:8000. Desktop browsers with keyboard and mouse only for now. Add `?stage=N` to the URL to start at stage N.

## License and attribution

Licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/): free to play, share and remix **non-commercially**, as long as you give credit and **link back to this repository**: https://github.com/nbwillcox/SpaceSidePews

This is an original game inspired by classic arcade shooters. It uses no assets, names or code from any existing game.
