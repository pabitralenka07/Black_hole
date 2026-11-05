# 🌌 3D Interactive Black Hole Simulation

An interactive, real-time 3D Black Hole and Accretion Disk simulation rendered with **Three.js** and custom **WebGL / GLSL shaders**. Experience the mesmerizing visual phenomenon of gravitational lensing, relativistic accretion disc dynamics, and thousands of particles spiraling into the event horizon.

---

## ✨ Features

- **🌀 Relativistic Accretion Disc**: High-fidelity procedural noise shader simulating the turbulent, superheated matter swirling around the black hole.
- **✨ Gravitational Lensing & Distortion**: Custom fragment shaders replicating the bending of spacetime and background light deflection around the singularity.
- **🌌 50,000+ Particle Inflow System**: GPU-accelerated particle engine modeling thousands of cosmic dust particles pulled past the photon sphere towards the event horizon.
- **⭐ Cosmic Starfield**: Deep-space background containing thousands of procedurally positioned and color-graded stars.
- **🎮 Interactive 3D Camera Controls**: Full 360° orbit, zoom, and pan controls powered by OrbitControls with smooth inertia and damping.
- **⚡ High Performance & Responsive**: Optimized WebGL rendering loop supporting dynamic pixel ratios and retina screens with 60+ FPS performance.
- **📦 Zero Build Configuration**: Pure static vanilla web stack (HTML5, CSS3, JavaScript) — runs seamlessly in any modern browser without npm dependencies or bundlers.

---

## 🚀 Live Demo & Preview

Open `index.html` directly in your browser or run via any static web server:

```
+-----------------------------------------------------------+
|                                                           |
|             .  *    .  *       .       *    .             |
|        .        *      .   :.:.:.:.  .        *           |
|      *      .        .  :::       :::   .        .        |
|                  .    ::             ::   *               |
|      .     *         ::   (  ⚫  )    ::       *    .      |
|                       ::             ::                   |
|         .       *      :::       :::      .        *      |
|      *      .           .  :.:.:.:.   .        .          |
|             .  *    .       .        *    .   *           |
|                                                           |
+-----------------------------------------------------------+
```

---

## 🛠️ Tech Stack

- **Rendering Engine**: [Three.js](https://threejs.org/) (WebGL 3D graphics)
- **Shaders**: Custom GLSL (OpenGL Shading Language) Vertex & Fragment Shaders
- **Language**: Vanilla JavaScript (ES6+)
- **Styling**: Modern CSS3 (Full-viewport fluid canvas)
- **Markup**: HTML5

---

## 📁 Project Structure

```bash
Black_hole/
├── index.html        # HTML entry point with canvas container
├── style.css         # Fullscreen responsive reset & viewport layout
├── script.js         # Three.js engine, GLSL shaders, particle simulation & controls
└── README.md         # Project documentation & guide
```

---

## ⚡ Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/pabitralenka07/Black_hole.git
cd Black_hole
```

### 2. Run Locally

You can simply open `index.html` in your favorite web browser, or serve it using any local HTTP server:

#### Using Python 3:
```bash
python3 -m http.server 8000
```
Then open `http://localhost:8000` in your browser.

#### Using Node.js (`npx serve` or `http-server`):
```bash
npx serve .
```

#### Using VS Code:
Right-click on `index.html` and select **"Open with Live Server"**.

---

## 🕹️ Controls

| Action | Control (Desktop) | Control (Touch/Mobile) |
| :--- | :--- | :--- |
| **Rotate View** | Left Click + Drag | Single Finger Drag |
| **Zoom In / Out** | Mouse Wheel Scroll | Two-Finger Pinch |
| **Pan Camera** | Right Click + Drag | Two-Finger Drag |

---

## 🔬 Scientific & Technical Details

### 1. Accretion Disc
The matter surrounding the black hole is rendered using procedural noise maps generated at runtime. The temperature and velocity gradient are expressed through smooth color transitions from fiery core hues (`#ff8080`) to outer cool tones (`#3633ff`).

### 2. Gravitational Lensing Mask
A dedicated post-processing render pass uses custom screen-space coordinates and radial distortion mapping to warp the background starfield around the black hole's photon sphere, mimicking Einstein's general relativity light deflection.

### 3. Particle Flow Physics
50,000 instanced particle points are assigned randomized orbital parameters, radius offsets, and speeds. An animation update loop calculates continuous angular displacement to visualize the accretion flow spiraling inward.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!
Feel free to check the [issues page](https://github.com/pabitralenka07/Black_hole/issues).

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
