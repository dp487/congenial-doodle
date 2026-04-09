# congenial-doodle

A stunning **3D Earth visualization** built with Three.js. This project creates a photorealistic, interactive Earth model with detailed surface textures, realistic atmospheric effects, cloud layers, and a starfield background. Perfect for showcasing 3D/WebGL skills and creative front-end development.

## 🎯 Features

- **Photorealistic Earth Model**: High-resolution textures for surface, specular highlights for water reflection, bump mapping for terrain detail, and night-time city lights
- **Atmospheric Glow**: Fresnel effect simulates realistic atmospheric scattering around Earth
- **Dynamic Cloud Layer**: Transparent, rotating cloud layer above Earth surface for lifelike appearance
- **Interactive Controls**: OrbitControls enable smooth rotation, zoom, and panning around the Earth
- **Starfield Background**: Procedurally generated starfield creates depth and space context
- **Responsive Design**: Adapts seamlessly across different screen sizes and aspect ratios
- **Realistic Rendering**: ACESFilmicToneMapping for cinematic color grading

## 🛠️ Tech Stack

- **3D Engine:** Three.js (WebGL)
- **Controls:** OrbitControls
- **Post-Processing:** EffectComposer, RenderPass, UnrealBloomPass (for atmospheric glow)
- **Textures:** Custom 4K+ resolution Earth textures (surface, specular, bump, night lights, clouds)
- **Rendering:** WebGLRenderer with tone mapping and color space management

## 📁 Project Structure

```
congenial-doodle/
├── index.html                    # Main HTML entry point
├── index.js                      # Main 3D scene setup and rendering
├── src/
│   ├── getStarfield.js          # Procedural starfield generation
│   └── getFresnelMat.js         # Fresnel effect material for atmospheric glow
├── textures/                     # Earth texture files (4K+)
│   ├── 00_earthmap1k.jpg        # Earth surface map
│   ├── 01_earthbump1k.jpg       # Bump mapping for terrain
│   ├── 02_earthspec1k.jpg       # Specular highlights (water reflection)
│   ├── 03_earthlights1k.jpg     # Night-time city lights
│   ├── 04_earthcloudmap.jpg     # Cloud layer
│   └── 05_earthcloudmaptrans.jpg # Transparent cloud layer
├── README.md                    # This file
└── package.json                  # npm dependencies (Three.js)
```

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- Optional: Node.js and npm (if using build tools)

### Installation

```bash
# Clone the repository
git clone <repository-url>
cd congenial-doodle

# Install dependencies (if package.json exists)
npm install
```

### Running

**Option 1: Direct HTML (No Build Required)**

```bash
# macOS
open index.html

# Windows
start index.html

# Linux
xdg-open index.html
```

**Option 2: HTTP Server (Recommended)**

```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve .

# Using PHP
php -S localhost:8000
```

Then open `http://localhost:8000` in your browser.

## 🎬 Demo

The visualization features:

- A photorealistic 3D Earth with realistic textures and atmospheric effects
- Rotating cloud layer for dynamic, living appearance
- Procedurally generated starfield for depth
- Smooth orbit controls for interactive exploration
- Responsive design that adapts to any screen size

## 🎨 Customization

### Textures

The `textures/` directory contains:
- `00_earthmap1k.jpg` - Earth surface map (daytime)
- `01_earthbump1k.jpg` - Bump mapping for terrain detail
- `02_earthspec1k.jpg` - Specular highlights for water reflection
- `03_earthlights1k.jpg` - Night-time city lights
- `04_earthcloudmap.jpg` - Cloud layer
- `05_earthcloudmaptrans.jpg` - Transparent cloud layer

Replace these with your own textures or higher resolution versions.

### Effects

Edit `index.js` to adjust:
- Cloud rotation speed
- Bloom effect strength
- Camera rotation speed
- Lighting and shadows

### Starfield

Edit `src/getStarfield.js` to customize:
- Star distribution
- Star brightness
- Starfield density

## 🧪 Future Work

- Add solar system toggle (show/hide other planets)
- Add real-time satellite tracking overlay
- Add weather pattern animations (storms, fronts)
- Add seasonal changes (tilt Earth axis for seasons)
- Add camera presets for famous locations
- Add VR/AR support (WebXR)
- Add web audio API for ambient space sounds
- Add time-lapse mode (day/night cycle)
- Add interactive data visualization (population, temperature, etc.)

## 📄 License

MIT
