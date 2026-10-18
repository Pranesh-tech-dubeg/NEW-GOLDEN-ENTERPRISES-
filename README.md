# NEW GOLDEN ENTERPRISES — Premium Architectural 3D Website

A luxury, minimalist architectural web application created for **NEW GOLDEN ENTERPRISES**, specializing in high-performance architectural windows, doors, and ventilation systems with dedicated interactive 3D studios.

---

## 🚀 How to Host on GitHub (Free & Instant)

This entire project is in **one self-contained folder** and is 100% ready to push to GitHub and deploy on GitHub Pages!

### Step 1: Create a New GitHub Repository
1. Log in to [GitHub](https://github.com/) and click **New Repository**.
2. Name it (e.g., `new-golden-enterprises`).
3. Leave it **Public** and do NOT initialize with README or .gitignore (they are already included).
4. Click **Create repository**.

### Step 2: Push This Folder to GitHub
Open a terminal (or VS Code terminal `Ctrl + ~`) inside this folder and run:

```bash
# 1. Initialize git
git init

# 2. Add all files
git add .

# 3. Create your initial commit
git commit -m "Initial commit: New Golden Enterprises 3D Architectural Website"

# 4. Set main branch
git branch -M main

# 5. Link to your GitHub repository (replace with your repo URL)
git remote add origin https://github.com/YOUR_USERNAME/new-golden-enterprises.git

# 6. Push code
git push -u origin main
```

### Step 3: Enable GitHub Pages
1. Go to your GitHub repository on github.com.
2. Click **Settings** (top tab) ➔ **Pages** (left sidebar).
3. Under **Build and deployment**:
   - **Option A (Automated GitHub Actions - Recommended)**:
     Set **Source** to **GitHub Actions**. The included `.github/workflows/deploy.yml` will automatically build and publish the site!
   - **Option B (Classic Branch Deploy)**:
     Set **Source** to **Deploy from a branch**, select branch **`main`**, folder **`/ (root)`**, and click **Save**.
4. In 1–2 minutes, your website will be live at:
   `https://YOUR_USERNAME.github.io/new-golden-enterprises/`

---

## 💻 Running Locally

### Option 1: Using Node.js (Included)
```bash
node server.js
```
Then visit: `http://localhost:3000`

### Option 2: Using VS Code Live Server
Right-click `index.html` and click **"Open with Live Server"**.

### Option 3: Using Python
```bash
python -m http.server 3000
```

---

## 📂 Project Directory Structure

```
Web Phase 1/
├── .github/
│   └── workflows/
│       └── deploy.yml           # Automated GitHub Pages deployment workflow
├── .vscode/
│   ├── launch.json              # VS Code debug launcher
│   └── settings.json            # VS Code workspace settings
├── assets/
│   └── images/
│       ├── hero/                # Architectural hero & craftsmanship photography
│       ├── products/            # Authentic production photos for all 8 window systems
│       └── projects/            # Real-world luxury architectural installations
├── css/
│   └── style.css                # Luxury architectural design system & responsive styling
├── js/
│   ├── main.js                  # Home page controller & scroll reveals
│   ├── product-detail.js        # Dedicated product page controller & switcher
│   ├── products-data.js         # Single source of truth database (8 products + pricing)
│   ├── three-scene.js           # Three.js 3D window engine (OrbitControls, zoom, animations)
│   └── vendor/
│       ├── three.module.js      # Three.js r160 core
│       ├── OrbitControls.js     # OrbitControls with trackpad scroll safety
│       └── GLTFLoader.js        # GLTF 3D model loader
├── .gitignore                   # Ignores node_modules, OS files, and logs
├── .nojekyll                    # Ensures GitHub Pages serves all JS modules and assets cleanly
├── index.html                   # Architectural home page with all 8 systems
├── package.json                 # Project configuration & npm scripts
├── product.html                 # Dedicated 3D studio (side-by-side view, pricing, colors, specs)
├── README.md                    # This guide
└── server.js                    # Zero-dependency local testing server
```

---

## 🏛️ Key Website Architecture

1. **Pure White & Champagne Gold Architectural Aesthetic**:
   - Pure `#FFFFFF` and `#F7F7F5` palette, satin champagne gold `#B99A5B` accents, and fine architectural borders `#E8E6E1`.
   - Typography: `Cinzel` & `Playfair Display` serif headings paired with `Plus Jakarta Sans` sans-serif UI.

2. **All 8 Systems with Dedicated 3D Studios**:
   - Every product card on `index.html` links directly to its dedicated studio page: `product.html?id=<product_id>`.
   - **01. Bathroom Ventilators**: Louvered ventilation + top-hung awning sash.
   - **02. Sliding Windows & Doors**: Multi-track panoramic sliding systems.
   - **03. Fixed Windows**: Ultra-slim 35mm sightline picture glass.
   - **04. French Windows & Doors**: Semicircular arched fanlights with sunburst muntins.
   - **05. Casement Windows**: Side-hung openable casements with breeze capture.
   - **06. Awning Windows**: Top-hung outward cantilever rain protection.
   - **07. Tilt-and-Turn Windows**: German dual-action inward turn and top tilt.
   - **08. Architectural Systems**: Bi-fold concertina folding glass doors.

3. **Side-by-Side 3D Customizer**:
   - **Left**: 3D interactive model with 360° rotation, physical sash operation animations, and toolbar with Zoom In `(+)` and Zoom Out `(-)` buttons.
   - **Right**: Fabrication pricing estimate (`₹/sq.ft`), 6 frame color swatches, 4 glass glazing options, and key engineering metrics.

4. **Laptop-Friendly Touchpad Experience**:
   - Mouse wheel and trackpad scroll hijacking is disabled by default, allowing natural, comfortable page scrolling on laptops without camera zoom trapping ("wildlife scrolling").

---

## 📱 Browser Compatibility
- Tested on Chrome, Safari, Firefox, Edge (Desktop, Tablet, and Mobile).
- Automatic WebGL fallback if hardware acceleration is disabled.
- 100% relative paths — zero server dependencies for static hosting.
