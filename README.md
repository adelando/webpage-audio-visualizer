# 🌈 AUDIO VISUALIZER V17.5.5

![Visualizer Header](https://img.shields.io/badge/Status-Stable-brightgreen)
![Visualizer Vers](https://img.shields.io/badge/Version-17.5.5-blue)
![VJ Ready](https://img.shields.io/badge/VJ-Ready-ff00ff)

A high-fidelity, browser-based audio reactive tool designed for live performances. Features an **Adaptive Spacing Engine** that maintains visual clarity regardless of line thickness.

---

## 🚀 Quick Start
1. **Open** the HTML file in any modern browser.
2. Click **System Audio Capture** (for internal sound) or **Microphone Input**.
3. If using System Audio, ensure the **"Share Audio"** toggle is enabled in the browser popup.
4. Press **F11** for the full-screen immersive VJ experience.

---

## 🎨 Effect Breakdown & Logic
Not every setting affects every shape. Use the table below to understand the unique behavior of each mode.

| Effect Name | Logic Description | Ignores These Settings |
| :--- | :--- | :--- |
| **🛰️ Orbiting Moons** | 400 stars orbiting a central point. Reacts by jumping outward from orbit. | Rotation Speed, Invert Toggle |
| **🍭 Kaleidoscope** | Mirrored bar patterns rotated around a central axis. | *Responds to all settings* |
| **🔺 Triangles** | Concentric geometric triangles pulsing to the bass. | *Responds to all settings* |
| **🔹 Hexagons** | Symmetrical 6-sided polygons with adaptive spacing. | *Responds to all settings* |
| **🔘 Circles** | Classic concentric rings. Best for "tunnel" effects. | *Responds to all settings* |
| **▪️ Squares** | Nested boxes. Great for architectural visuals. | *Responds to all settings* |
| **📊 Mirror Bar** | Traditional frequency bars mirrored on the X-axis. | **Rotation Speed, Invert Toggle** |
| **🔉 Waveform** | Direct time-domain representation of the audio signal. | **Invert Toggle, Complexity** |

---

## 🎛️ Control Manual

### **Core Rendering**
* **Gain / Sensitivity:** Multiplier for the audio input. Turn up for quiet tracks.
* **Base Spacing:** Sets the initial gap between shapes/bars.
* **Line Thickness:** Controls the width of the lines. 
    * *Note: Includes a dynamic buffer ($Spacing + (Thickness \times 1.5)$) to prevent overlapping.*
* **Complexity:** Determines how many rings or kaleidoscope slices are rendered.
* **Rotation:** The speed at which the entire canvas spins.
* **Master Zoom:** Overall scale of the visual.
* **Decay (Trails):** Controls how long previous frames linger. Low = High Blur; High = Sharp Lines.

### **Color & Style**
* **Color Mode:** Choose between Rainbow or 5 specialized palettes (Cyberpunk, Lava, etc.).
* **Custom Palette:** Allows you to pick two specific colors to blend between.
* **Color Speed:** How fast the hues cycle through the spectrum.

---

## 🎹 Pro VJ Shortcuts
The visualizer is built for live performance. Use your keyboard for instant transitions:

* **[1] through [9]:** Instantly load the corresponding Preset Slot.
* **[⚙️ Icon]:** Click to hide/show the UI panel for a clean recording.

---

## 💾 Data Management
* **Preset Bank:** 9 slots of local storage that persist even if you refresh the page.
* **Export:** Converts your current masterpiece into a Base64 string. Share this code with others!
* **Import:** Paste a code into the box to instantly replicate someone else's setup.

---

## 🛠️ Project Goals
Created by **Adelando**, this project aims to provide a zero-latency VJ solution that requires no software installation. 

**Future Roadmap:**
* [ ] Mobile-specific touch gestures?
* [ ] Frequency range isolation (Low/Mid/High focus)?

**Found a bug?** Open an issue on the [GitHub Repository](https://github.com/adelando/webpage-audio-visualizer).
