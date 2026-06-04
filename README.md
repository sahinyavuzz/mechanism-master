# Mechanism Master

A physics-based mechanism design puzzle game. Design four-bar linkages whose coupler points trace target curves drawn from real mechanical engineering principles.

**Status:** Early prototype (v0.1) · Seeking player feedback

---

## Play

Open the game in your browser: **[Play Mechanism Master](https://sahinyavuzz.github.io/mechanism-master/)**

Works on desktop and mobile. No installation required.

---

## How it Works

Each level presents a target curve drawn as a red dashed line — this is the path a point on the coupler link must trace. You design the four-bar linkage by adjusting:

- **Link lengths** (r₂ crank, r₃ coupler, r₄ rocker) — the ground length r₁ is fixed per level
- **Coupler point position** — distance from joint A, and angle relative to coupler AB

As you adjust parameters, the mechanism simulates in real time and traces its path in blue ink. Match your trail to the target with 70% or better accuracy to clear the level.

The Grashof condition is shown in real time: if it fails, the crank cannot fully rotate and the mechanism oscillates — adding a hidden engineering constraint to the puzzle.

---

## About

Created by **Prof. Dr. Şahin Yavuz**, Department of Mechanical Engineering, Dokuz Eylül University, Türkiye.

Built to explore whether real mechanical engineering principles — four-bar linkage kinematics, Grashof's theorem, coupler curve theory — can power compelling puzzle gameplay accessible to a wide audience. Inspired by *Poly Bridge*, *Kerbal Space Program*, and *Opus Magnum*.

The mathematics under the hood is the same kinematic analysis taught in mechanism design courses. The simulation solves the position equations exactly (intersection of two circles) at 60 frames per second.

---

## Feedback

If you played the game, your feedback would be invaluable. Tell me:

- Which level frustrated you most? Which felt rewarding?
- Did the controls make sense?
- Would you play more levels? Would you pay for a polished version?
- Any bugs, glitches, or strange behavior?

[Open an issue](https://github.com/sahinyavuzz/mechanism-master/issues/new) or comment on the [discussions tab](https://github.com/sahinyavuzz/mechanism-master/discussions).

---

## License

Copyright © 2026 Şahin Yavuz. All rights reserved.  
See [LICENSE.txt](LICENSE.txt) for full terms.

This is proprietary software. Reproduction, modification, distribution, or commercial use without written permission is prohibited.

---

*Built with care in İzmir, Türkiye.*
