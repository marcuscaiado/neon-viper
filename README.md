# 🐍 Neon Viper 3D ✨ — Cyber Slither Arena

[![Live Demo](https://img.shields.io/badge/🎮_Play_Live_Demo-marcuscaiado.github.io-success?style=for-the-badge&logo=githubpages&logoColor=white)](https://marcuscaiado.github.io/neon-viper/)
[![Three.js](https://img.shields.io/badge/WebGL_3D-Three.js_r128-00f5ff?style=flat&logo=three.js&logoColor=white)](https://threejs.org/)
[![Arcade Hub](https://img.shields.io/badge/🕹️_Arcade_Hub-Connected-05ffa1?style=flat)](https://marcuscaiado.github.io/marcus-arcade/)
[![60 FPS](https://img.shields.io/badge/Performance-60_FPS_Mobile_&_PC-ffd700?style=flat)](https://marcuscaiado.github.io/neon-viper/)

A high-octane 3D **Snake.io** cyber battle arena featuring realistic 3D perspective camera follow, 8 customizable snake skins, lethal electric perimeter walls, classic self-collision, and High-IQ competitive AI bots!

---

## 🎮 Play Online
👉 **[https://marcuscaiado.github.io/neon-viper/](https://marcuscaiado.github.io/neon-viper/)**

---

## ⚡ Recent Major Updates

### 💥 100% Precise Instant Collision Death
- **0.0s Spawn Delay**: Zero artificial grace period for the player — instant lethal response!
- **Lethal Electric Boundary Wall**: The glowing 3D perimeter cylinder is a live electric forcefield. Touching it (`headRadius + dist >= ARENA_RADIUS`) immediately triggers a catastrophic explosion!
- **Classic Self-Collision (Don't Touch Yourself!)**: Biting or crossing into your own tail (from segment 5+ backwards) triggers an instant explosion with floating message: `"Your viper bit its own body and exploded 💥"`.
- **3D Neon Particle Explosion Sparks**: Dying shoots 35-45 colorful 3D physics sparks that bounce across the arena floor, backed by a heavy sub-bass explosion sound effect.

### 🧠 High-IQ Competitive AI Bots (No More Dumb Suicides!)
- **5-Direction Whiskers Feeler Probing**: Bots cast forward lookahead rays ($0^\circ, \pm 26^\circ, \pm 51^\circ$) across 38 units to evaluate spatial clearance.
- **Self-Body Clearance Awareness**: Bots actively track their own body trails, completely preventing self-tail bites and accidental self-coiling suicides.
- **Perimeter Safety Curving**: When within 40 units of the arena edge, bots smoothly steer back toward the center, eliminating wall collisions.
- **Predatory Cut-Offs**: When hunting smaller snakes (including the player), competitive bots calculate lead intercept vectors and fire tactical nitro bursts to cut them off!
- **Defensive Evasion**: Bots flee and nitro away when larger snakes threaten their heads.

---

## ✨ Features & Highlights

- **3D Perspective Slither Arena**: Powered by Three.js WebGL with dynamic camera follow that smoothly zooms out as your viper grows into a massive titan.
- **Screen-Relative Vector Steering**: Deadzone protection prevents death-spin glitches; snake glides smoothly along your mouse or touch vector.
- **8 Custom 3D Snake Skins**:
  1. 🐍 **Neon Viper**: Signature cyan/emerald cyber serpent with glowing dorsal spine.
  2. 🐲 **Mecha Dragon**: Titanium plating with gold/orange energy thrusters.
  3. 🌌 **Cosmic Void**: Deep nebula violet with star-sparkle aura.
  4. 🌈 **Hyper Rainbow**: Real-time chromatic shifting rainbow spectrum.
  5. 🌋 **Molten Magma**: Volcanic obsidian with glowing lava veins.
  6. 🌸 **Sakura Glaze**: Pearlescent pastel pink and soft anime dragon eyes.
  7. 👑 **Golden King**: 24K mirror gold chrome with a floating royal crown.
  8. 💻 **Matrix Cyber**: Deep cybernetic green with digital circuitry patterns.
- **3D Cartoon Fruits & Orchard**: Consumable Watermelons (35 pts), Strawberries, Apples, Oranges, Bananas & Grapes with 5-second freshness decay timers.
- **Arcade Hub Sync**: Classic 3-letter initials pilot tag (`MRC`) and global high-score sync.

---

## 🕹️ Controls

| Action | Desktop / Keyboard | Mobile / Touchscreen |
| :--- | :--- | :--- |
| **Steer Viper** | Move Mouse Cursor | Drag / Touch anywhere on screen |
| **Nitro Boost** | Hold Left Click or `[SPACE]` | Hold **NITRO BOOST** Button |
| **Change Skin** | Click `🎨 Skins` in top bar | Tap `🎨 Skins` in top bar |

---

## 🛠️ Tech Stack

- **Three.js (r128)** — 3D arena cylinder, procedural snake mesh segments, dynamic lighting.
- **Web Audio API** — Synthesized eating chimes, nitro hums, and heavy sub-bass explosion crashes.
- **Universal Arcade Leaderboard** — Global leaderboard sync.
