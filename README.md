# The Daily Grind ☕⚡
> A tactile, kinetic barista shuffleboard and merge puzzle game built with zero external dependencies and optimized for iOS Safari, Android, and Desktop.

Inspired by tabletop shuffleboard, curling, and physics merge puzzles, **The Daily Grind** places players behind a café prep counter. Instead of dropping items under gravity, players aim, power up, and slide craft coffee pucks across a frictionless counter surface. Collide matching items to trigger merge bursts, carom off stainless steel bumpers, and clear space to reach the ultimate apex mood brew—**Litta**.

---

## 🕹️ Gameplay & Mechanics

### Level Plane Shuffleboard Physics
* **Zero Gravity / Top-Down View:** The game takes place on a level café counter surface. 
* **Tactile Slide & Flick:** Touch or click the ready puck in the launch lane. Drag to calibrate angle and sliding velocity, then release to push the puck across the bar.
* **Surface Drag & Momentum Transfer:** Moving pucks encounter kinetic counter friction and gradually decelerate, knocking stationary ingredients forward and sideways into strategic clusters.
* **Side Bumper Rebounds:** Carom pieces off the side guardrails to weave past congested center lanes.
* **Foul Line Rule:** If a puck is deflected or rebounded back across the launcher foul line, or if the prep lane clogs up, the shift ends.

---

## ☕ Craft Merge Progression

Combine two identical items to trigger a merge burst and advance up the barista craft tiers:

| Tier | Item | Base Points | Mass Multiplier | Visual Marker |
| :---: | :--- | :---: | :---: | :---: |
| **1** | Raw Green Bean | 4 pts | $1.0\times$ | 🌱 Green |
| **2** | Roasted Bean | 8 pts | $1.4\times$ | 🟤 Dark Roast |
| **3** | Ground Coffee Puck | 16 pts | $2.1\times$ | ☕ Puck |
| **4** | Crema Espresso Shot | 32 pts | $3.0\times$ | ✨ Golden Crema |
| **5** | Steamed Oat Foam | 64 pts | $4.2\times$ | 🥛 Microfoam |
| **6** | Flat White | 128 pts | $5.6\times$ | 🫖 Ceramic Cup |
| **7** | Iced Cold Brew | 256 pts | $7.2\times$ | 🧊 Tumbler |
| **8** | **The Litta Can (Apex)** | 512 pts | $9.5\times$ | ⚡ Functional Mood Can |

---

## 🏆 Barista Shifts (Dynamic Counter Upgrades)

As your score accumulates, the café upgrades the prep counter surface with new dynamic friction and rebound properties:

* **Shift 1: Marble Prep Counter ($0\text{–}349\text{ pts}$):** Standard counter surface friction ($\mu = 0.982$) with moderate bumper rebound ($e = 0.55$).
* **Shift 2: Polished Stainless ($350\text{–}899\text{ pts}$):** Low-friction speed surface ($\mu = 0.989$) with elastic, bouncy rebounds ($e = 0.65$).
* **Shift 3: Speed Rail Rush ($900+\text{ pts}$):** Near-frictionless glide ($\mu = 0.993$) requiring featherlight flick control and high-speed caroms ($e = 0.72$).

---

## 📱 Cross-Platform Support & PWA Installation

The game engine is tuned specifically to overcome mobile browser constraints (including iOS Safari touch-cancelling and gesture-swallowing).

### iPhone & iPad (iOS Safari)
1. Open the game link in **Safari**.
2. Tap the **Share** button (box with an upward arrow) in the Safari toolbar.
3. Scroll down and select **"Add to Home Screen"**.
4. Confirm by tapping **Add**. The game will launch full-screen in standalone display mode without URL address bars.

### Android (Google Chrome)
1. Open the game link in **Chrome**.
2. Tap the three-dot menu (**⋮**) in the upper-right corner.
3. Select **"Install app"** or **"Add to Home screen"**.

### Mac & Desktop PC
* **macOS (Safari):** Select **File > Add to Dock** to install it as an isolated desktop window.
* **Chrome / Edge:** Click the **Install** icon on the right side of the URL bar.

---

## 📁 Repository Structure

```text
├── TheDailyGrind.html    # Standalone, zero-dependency game file
├── README.md             # Project documentation and deployment guide
└── ...
```

---

## 🚀 Deployment & Local Testing

### Quick Local Preview
Run any static local web server inside the repository folder:

```bash
# Using Python
python3 -m http.server 8080

# Using Node.js
npx serve .
```
Navigate to `http://localhost:8080/TheDailyGrind.html` in your browser.

### Deploying to GitHub Pages
1. Push `TheDailyGrind.html` to your GitHub repository (you can rename it to `index.html` to serve it at the root).
2. Go to **Settings > Pages** in your repository.
3. Under **Branch**, select `main` (or `master`) and folder `/(root)`.
4. Click **Save**. GitHub Pages will deploy the project over HTTPS, enabling the web app install prompt for iOS and Android devices.

---

## 📄 License & Attribution
Designed for educational and prototyping purposes. Inspired by modern casual merge puzzles and functional mood coffee branding concepts.