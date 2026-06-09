# Beehive Prototype — DTL Visualiser

## Overview
This is a fully interactive, procedurally generated 3D visualisation of the **Safe Inspection & Feeding Upgrade** module for traditional ISI standard beehives. It was built as a single, self-contained HTML file using **Three.js** (`r165`).

The application renders the entire hive procedurally—there are no external 3D models or texture image files to load. All wood grains, materials, and geometries are generated using JavaScript via the HTML5 Canvas API and Three.js primitives.

## Key Features & Upgrades

### 1. ISI Standard Foundation
The core dimensions are based on the Bureau of Indian Standards (ISI) for *Apis mellifera* (Langstroth-based):
*   **Floor Board**: Extended landing board (60mm)
*   **Brood Box (Empty)**: 505 x 405 x 245 mm external. The traditional brood frames have been removed in this visualiser to clearly showcase the interior upgrades.
*   **Super Chamber**: 150mm height, adapted for shorter Flow frames.
*   **Bee Space**: Maintained at exactly 9mm throughout the design.
*   **Telescoping Roof**: Features a metal (tin) top with bent edges and ventilation holes.

### 2. Internal Insulation Upgrade
*   Thin (10mm) XPS insulation is integrated directly onto the inner walls of the brood box.
*   It covers the left, right, and back walls.
*   The front wall insulation has been intentionally omitted to ensure proper ventilation and clear access to the bottom entrance.

### 3. Dual Safe Inspection Windows
To allow beekeepers to inspect the colony without disturbing the internal temperature or risking defensive behavior:
*   **Left Wall Window** (200 × 140 mm)
*   **Back Wall Window** (180 × 120 mm, offset 80mm to the right)
*   Both windows feature an inner clear **acrylic glass panel**.
*   A routed MDF recess frame and **silicone bead** ensures an airtight seal.
*   External sliding **wooden shutters** (sliding sideways along their respective walls) block light when not inspecting.
*   A physical **bee-space indicator (9mm)** is printed directly onto the acrylic to help assess if comb is being drawn too close to the glass.

### 4. Top Feeding Mechanism
A redesigned feeding system to feed bees without opening the hive:
*   **External Funnel**: Mounted on the upper right side of the super exterior.
*   **Feed Tube**: Channels the syrup horizontally through the wooden wall.
*   **Internal Tray**: Sits securely inside the super, above the flow frames. 
*   **Visualisation**: The inner cover (crown board) is semi-transparent, allowing you to see the feeder tray from above. The UI includes an animated "Show Feeding" mode with simulated dripping syrup.

### 5. Flow Harvesting (Front Spout)
*   Equipped with 7 shortened (340mm) Flow-style harvesting frames.
*   Harvest mechanism has been rerouted so the **harvest spout exits from the front** of the super, directing the honey flow forward.
*   Animated "Activate Harvest" mode simulates cell splitting and honey dripping from the spout.

## Interactive UI Controls
The application features a dark-glass UI panel at the bottom left with the following controls:
*   **Open/Close Shutter**: Slides both the left and back window shutters open.
*   **Activate Harvest**: Simulates the flow hive harvesting process.
*   **Show Feeding**: Animates syrup flowing through the funnel and tube into the internal tray.
*   **Visibility Toggles**: Hide/show the internal Insulation, Flow Super box, internal Flow Frames (separately from the super box), Top Feeder, and Roof.
*   **Exploded View**: Disassembles all the hive components vertically and laterally to show how they fit together.

## Camera System
Top right presets allow for quick navigation:
*   **Default**: Isometric front-right view.
*   **Front**: Direct view of the entrance and harvest spout.
*   **Back**: Direct view of the rear inspection window.
*   **Left**: Direct view of the left inspection window.
*   **Top**: Bird's-eye view (great for seeing the feeder tray through the transparent cover).
*   **Window**: Zooms in very close to the left inspection window.
*   **Orbit**: Toggles a smooth, automatic 360° rotation around the hive.

## How to Run

Because the application uses ES modules (`type="module"`) to import Three.js, it **must** be served over a local web server (opening the file directly via `file:///` will result in CORS block errors).

1. Open your terminal in this directory (`04-prototype`).
2. Start a simple Python HTTP server:
   ```bash
   python -m http.server 8765
   ```
3. Open your web browser and navigate to:
   [http://localhost:8765/beehive-prototype.html](http://localhost:8765/beehive-prototype.html)
