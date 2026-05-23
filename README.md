# AI Travel Planner - Immersive 3D WebGL Dashboard

A premium, award-winning **3D WebGL interactive travel portal** built with **Three.js** (loaded via CDN) and standard CSS 3D transforms. This immersive static single-page app serves as the human-in-the-loop review interface for your multi-agent travel orchestrator backend.

---

## 3D WebGL Visual Highlights

- **Procedural 3D Earth Particle Globe**: Renders a glowing Earth sphere made of 5,500 interactive indigo stars. Placed via live coordinate sampling of an in-memory procedural continent canvas, ensuring zero asset-loading lag and absolute standalone reliability.
- **Atmospheric Wireframe Aura**: Features a slightly larger, translucent ambient halo sphere simulating atmospheric thickness.
- **Drift Starfield Parallax**: Generates a deep cosmos background of 2,500 random twinkling starry particles drifting in the opposite orbit.
- **Direct Orbit Drag Controls**: Built with lightweight, custom WebGL drag listeners that translate mouse/touch movement into smooth multi-axis planetary rotation.
- **Glowing Flight Curve Vectors**: Triggering a destination query generates a pulsing beacon indicator and sweeps a glowing quadratic Bezier 3D curve (flight path arc) on the globe.
- **AI Orbit Acceleration Nodes**: The globe accelerates its rotation dynamically during API background polling, visually representing the AI specialists assembling the research and itinerary datasets.
- **3D Parallax Day Tilts**: Day itinerary accordion cards tilt dynamically in 3D in response to mouse coordinate movements, displaying glowing neon shadows that track your cursor.
- **Settings Panel Removed**: Removed all server configuration settings, locking all fetch routes securely to your live backend endpoint: `https://ai-travel-planner-gmhq.onrender.com`.

---

## Quick Setup & Run

No bundlers or npm server-side installs are needed.

### 1. Locally
Open the `index.html` file directly in any modern web browser!

Alternatively, spin up a simple static web server:
```bash
python -m http.server 3000
```
Then visit: `http://localhost:3000`

### 2. Live Deployment
Since this repository consists purely of static assets (`index.html`), it is extremely fast and free to deploy on:
- **Vercel** (Preset: `Other`, Root: `./`, Build and Output: default/blank)
- **Netlify**
- **GitHub Pages**
