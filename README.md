# PI-SECT (`pi-sect`)

**1D & 2D Quadtree Time-Attack Binary Search Arcade Game**

👉 **Play Live:** [https://talsheaffer.github.io/pi-sect/](https://talsheaffer.github.io/pi-sect/)

---

## 🎮 Overview

**PI-SECT** is an infinite-precision reflex arcade game built on binary search (1D) and quadtree subdivision (2D). Using a custom 320-decimal-digit `BigInt` coordinate engine, you can zoom into irrational numbers ($\pi, \phi, \sqrt{2}, \sqrt{3}$, or fresh 320-digit points) past $2^{1000}\times$ magnification without ever hitting 64-bit floating-point underflow.

### Key Features
- **1D Line & 2D Quadtree Modes**: Slice a 1D interval into Left/Right halves or a 2D plane into `NW` / `NE` / `SW` / `SE` quadrants.
- **320-Digit `BigInt` Engine**: Watch decimal digits lock in as your interval bounds converge on $\pi$, $\phi$, $(\pi, \phi)$, $(\sqrt{2}, \sqrt{3})$, or a random irrational target.
- **Zero-Eye-Travel Urgency Cues**: A synchronized collapsing ring and radial halo around the target orb shift smoothly from **Cyan → Amber → Crimson** as the step clock counts down.
- **3-Life Shield System**: Survive timeouts or misclicks with up to 3 lives per run.
- **Web Audio Synthesizer**: Dynamic pitch-escalating triangle/sawtooth synth feedback on every slice.

---

## ⌨️ Controls

| Mode | Action | Keyboard Shortcuts | Mouse / Touch |
| :--- | :--- | :--- | :--- |
| **1D Line** | Bisect Left `[0, 0.5)` | `←` or `A` | Click/tap left half of canvas or **BISECT LEFT** button |
| **1D Line** | Bisect Right `(0.5, 1]` | `→` or `D` | Click/tap right half of canvas or **BISECT RIGHT** button |
| **2D Quadtree** | Top-Left (`NW`) | `Q` or `7` | Click/tap top-left quadrant or **NW Quad** button |
| **2D Quadtree** | Top-Right (`NE`) | `W`, `E`, or `9` | Click/tap top-right quadrant or **NE Quad** button |
| **2D Quadtree** | Bottom-Left (`SW`) | `A` or `1` | Click/tap bottom-left quadrant or **SW Quad** button |
| **2D Quadtree** | Bottom-Right (`SE`) | `S`, `D`, or `3` | Click/tap bottom-right quadrant or **SE Quad** button |
| **Any** | Restart Run | `R` (or `Space` on Game Over) | Click **Restart [R]** |

---

## 🛠️ Local Development

Because `pi-sect` has zero build dependencies, you can run it locally with any static server or hot-reload dev server:

```bash
# Option A: Instant live-reload on save via Vite
npx vite

# Option B: Python built-in HTTP server
python3 -m http.server 8000
```
