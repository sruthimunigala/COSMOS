# 🪐 COSMOS: Beyond Horizons — Interactive 3D Universe & Space Explorer

**COSMOS: Beyond Horizons** is an interactive 3D WebGL web platform built with Three.js that simulates the Solar System, moons, asteroids, comets, and deep space phenomena. It features realistic procedural textures, cinematic relativistic hyperdrive travel, planetary size and void distance comparisons, an intelligent conversational AI guide with voice synthesis, and an upcoming real-world space events and skywatching calendar.

---

## 🌟 Key Features

### 1. 🌌 Interactive 3D Universe & Beyond
- **Central Sun**: High-energy solar granulation procedural shader with glowing corona halos and dynamic point lighting.
- **The 8 Major Planets & Pluto**: Mercury, Venus, Earth (with rotating cloud layer and atmospheric glow), Mars, Jupiter (with Great Red Spot), Saturn (photorealistic procedural rings with Cassini division), Uranus (axial tilt of 98° and vertical rings), Neptune, and Pluto.
- **Moons & Ocean Worlds**: Earth's Moon, Io (volcanic sulfur), Europa (ice shell and subsurface oceans), Ganymede, Callisto, Titan (liquid methane oceans and nitrogen smog), Enceladus (cryovolcanic geysers), and Triton (retrograde orbit).
- **Asteroids & Protoplanets**:
  - Instanced Asteroid Belt of 2,200+ tumbling asteroids with realistic Kirkwood gaps.
  - Ceres (dwarf planet), Vesta, 16 Psyche (metal core worth $10,000 quadrillion), Bennu, and Apophis (2029 close pass).
- **Comets & Interstellar Visitors**:
  - 1P/Halley, C/2020 F3 (NEOWISE), and 1I/'Oumuamua with dynamic dual ion (blue anti-solar) and dust tails.
- **Deep Space Sector**:
  - Voyager 1 & 2 escape trajectories into interstellar space.
  - Proxima Centauri red dwarf neighbor star.
  - Orion Nebula stellar nursery.
  - Sagittarius A* Supermassive Black Hole with relativistic Doppler-beamed accretion disk and photon sphere.

### 2. 🚀 Cinematic Navigation & Relativistic Travel
- **Warp Drive Effect**: Fullscreen radial warp streak stars and FOV expansion during travel between celestial bodies.
- **Target Tracking & Orbital Lock**: Camera locks onto planets and dynamically follows them along their orbits while allowing complete 360° rotation.
- **Camera Presets**:
  - **Free Orbit Mode**: Drag to rotate, scroll to zoom, right-click to pan.
  - **Top-Down Overview**: Polar heliocentric perspective of the entire solar system and planetary orbits.
  - **The Grand Tour**: Automated cinematic autopilot navigating through the cosmos with guided checkpoints.

### 3. ⚖️ Planetary Scale & Distance Void Simulator
- **Cosmic Lineup**: Side-by-side true scale comparison between any two celestial bodies.
  - Real radius ratio, volume multiplier ("How many Earths fit inside Jupiter"), exterior surface area, and relative surface gravity.
- **Cosmic Void Simulator**:
  - Speed of light travel-time calculator (e.g. Earth to Jupiter = 43 minutes).
  - Interplanetary travel durations for spacecraft (50,000 km/h) and commercial jetliners (900 km/h).

### 4. 🤖 "COSMOS AI" Guide (Astrobiology & Flight Officer)
- **Context-Aware Responses**: AI recognizes the currently visited celestial body and provides real-time telemetry.
- **Autonomous Simulation Commands**:
  - "Fly to Saturn" -> AI executes warp drive to Saturn!
  - "Compare Earth and Jupiter" -> Launches comparison modal!
  - "Show upcoming space launches" -> Opens events calendar!
  - "Top-down view" -> Switches camera to polar overview!
  - "Start Grand Tour" -> Launches automated cosmic tour!
- **Text-to-Speech (TTS) Voice Synthesis**: Voice narration with animated audio visualizer wave.

### 5. 📅 Upcoming Space Events & Skywatcher Calendar
- Curated timeline of upcoming real-world milestones (2024–2029+):
  - **Rocket Launches**: NASA Artemis II, Artemis III, SpaceX Starship Orbital Refueling, Dragonfly to Titan.
  - **Celestial Phenomena**: Great European Total Solar Eclipse (2026), Perseid and Geminid meteor showers.
  - **Deep Space Missions**: Europa Clipper Jupiter arrival, Asteroid Apophis close flyby (2029).
- **Live Countdown Clock**: Days, hours, minutes, and seconds to the next major milestone.
- **Viewing & Telemetry Guides**: Naked-eye, binocular, and telescope recommendations.
- **Event Simulation**: One-click alignment simulator for eclipses and orbit insertions.

### 6. 🎵 Procedural Web Audio Engine
- Ambient deep-space synthesizer drone generated dynamically using the Web Audio API (zero external audio files).
- Sci-fi warp drive frequency sweeps and holographic telemetry UI chimes.

---

## 🕹️ Keyboard Controls & Shortcuts

| Key | Action |
|---|---|
| `Space` | Pause / Resume Orbital Simulation Time |
| `T` | Polar Heliocentric Top-Down View |
| `R` | Reset Camera to Default Perspective |
| `M` | Mute / Unmute Procedural Sound Engine |
| `Esc` | Close Open Modals / Dossier Drawer |

---

## 💻 Running the Website

### Option 1: Quick Launcher (Windows)
Double-click `start.bat` in the project root folder.

### Option 2: Command Line
```bash
agy-node server.js
```
Then open your browser at:
```
http://localhost:3000
```

---

## 📁 Project Architecture
```
d:\cosmos\
├── index.html                 # Main entrypoint with aerospace HUD layout
├── css/
│   ├── main.css               # Cyberpunk/aerospace styling, glassmorphism, animations
│   └── responsive.css         # Mobile and tablet viewport optimizations
├── js/
│   ├── config.js              # Astronomical data, physical constants, events, AI knowledge
│   ├── textures.js            # Procedural canvas textures (planets, rings, sun, clouds, black hole)
│   ├── solarSystem.js         # Three.js scene, orbits, lighting, stars, asteroid belt, comets
│   ├── cameraManager.js       # Warp speed effects, fly-to tweening, orbital tracking, grand tour
│   ├── scaleComparison.js     # Planetary size comparison & distance void calculators
│   ├── aiGuide.js             # COSMOS AI conversational agent & voice speech synthesizer
│   ├── eventsCalendar.js      # Filterable space events schedule and live countdown clocks
│   ├── audioManager.js        # Procedural Web Audio space ambient synthesizer & SFX
│   └── main.js                # Bootstrap, search autocomplete, drawers, hotkeys, UI events
├── vendor/
│   ├── three.min.js           # Three.js 3D WebGL engine
│   ├── OrbitControls.js       # Camera orbit and touch controls
│   └── tween.umd.js           # Smooth cinematic motion interpolation
├── server.js                  # Standalone local HTTP server
└── start.bat                  # One-click launcher script
```
