[thumbtak_arcade_readme.md](https://github.com/user-attachments/files/35002910/thumbtak_arcade_readme.md)
# 🕹️ ThumbTak Arcade

**Rapid Thumbnail & Ad Creative Ideation, Swipe Triage, and Budget Voting — Built as a Single-File Retro Arcade Web App.**

ThumbTak helps YouTube creators, performance marketers, and creative teams generate high-volume visual concepts, stress-test their layouts on tiny mobile screens, and pick top performers using bias-mitigated **$100 play-money voting** and **real pixel-level contrast checks**.

---

## ✨ Key Features

### 1. High-Volume Concept Generation
* **One-Click Platform Presets:** Instantly configure aspect ratios and batch sizes for **YouTube (`16:9`)**, **Meta / Instagram (`4:5`)**, **Shorts / TikTok (`9:16`)**, or **Storyboards (`24 frames`)**.
* **Prompt-Aware Visual Engine:** Parses subjects, materials (copper, gold, glass, wood, neon, wire sculptures), and environments directly from your brief.
* **Seed Photo & Sketchpad Blending:** Upload a reference thumbnail or draw rough composition shapes on the built-in **Sketch Pad** to guide generated variations.
* **"8 Like This" Branching & Remixing:** Evolve 8 new variations from any promising card, or cycle through layout remixes (`Swap Subject`, `Mix Layouts`, `Zoom In Big`, `Remove Clutter`, `Invert Colors`).
* **Real AI Favorites Rendering:** Upgrade starred concepts into full AI-rendered images via Gemini (`gemini-3.1-flash-image`).

### 2. Arcade Swipe Triage & Layout Checks
* **Card Judge Swipe Queue:** Rapidly triage 8 to 100 generated ideas with mouse drag, touch gestures, or keyboard shortcuts (`←` Pass, `→` Keep, `Z` Rewind/Undo).
* **8-Minute Crazy 8s Sprint Timer:** Built-in countdown clock to keep ideation fast and prevent overthinking.
* **Tiny Phone Check:** Shrinks the contact sheet to mobile-feed scale in high-contrast greyscale to verify whether focal points and silhouettes read at a glance.
* **Flip Left/Right (Mirror Check):** Flips thumbnails horizontally to break visual habituation and expose lopsided compositions.
* **On-Canvas Headline Overlays:** Toggle bold, high-contrast text badges directly on cards and export high-res `1080×1080` PNGs with typography burned in.

### 3. Bias-Mitigated Selection & Export
* **$100 Budget Vote:** Allocate $100 in mock currency across your starred finalists to force real trade-offs instead of starring everything.
* **Shareable Voting Links:** Encodes starred finalists directly into the URL hash (`#vote=...`) so teammates or clients can open the link and vote immediately.
* **Live Feed & Pixel Contrast Telemetry:** Measures real center-vs-edge luminance contrast and 120px legibility on an offscreen `<canvas>`, then previews your Top 3 side-by-side in a crowded YouTube/Social scroll mockup.
* **Social Poll & Production Exports:** Download a ready-to-post **`A / B / C` Poll Graphic**, print a **1-Page Brief PDF**, or copy a **Figma & Ad Rotation JSON** manifest.

---

## 🚀 Getting Started

ThumbTak Arcade is a **zero-dependency, single-file web application** (`index.html`). No build tools, Node.js, or package installations are required.

1. **Clone or download** this repository.
2. **Open `index.html`** directly in any modern web browser (Chrome, Edge, Safari, or Firefox).
3. *(Optional)* To enable **Render Real AI Favorites**, add your Gemini API key inside `upgradeFavoritesWithRealAI()` in `index.html`:
   ```javascript
   const apiKey = "YOUR_GEMINI_API_KEY";
   ```

---

## 🎮 Keyboard Shortcuts (Card Judge)

| Key | Action |
| :--- | :--- |
| `→` (Right Arrow) | **Keep / Star** current card |
| `←` (Left Arrow) | **Pass** current card |
| `Z` | **Rewind / Undo** previous swipe |
| `Esc` | **Exit** Card Judge back to the grid |

---

## 🛠️ Tech Stack

* **HTML5 & Vanilla JavaScript** (single-file architecture)
* **Tailwind CSS** (via CDN)
* **HTML5 `<canvas>` & SVG** (procedural scene rendering, sketchpad input, offscreen contrast analysis, and PNG/poll graphic export)
* **Web Audio API** (synthesized 8-bit arcade sound effects with zero external audio assets)

---

## 📄 License

MIT License — free to use, modify, and distribute.
