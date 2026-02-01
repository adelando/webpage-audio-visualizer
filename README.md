# 🌈 CHROMIUM WEB AUDIO VISUALIZER

![Visualizer Header](https://img.shields.io/badge/Status-Stable-brightgreen)
![Visualizer Vers](https://img.shields.io/badge/Version-17.5.5-blue)
![VJ Ready](https://img.shields.io/badge/VJ-Ready-ff00ff)

*Wish spotify, Apple Music or Youtube Music had a fullscreen visualizer for your party or event?*

A high-fidelity, browser-based, audio reactive tool designed to produce amazing visuals, that are extremely customisable.  
Features a <ins>**Preset Manager**</ins> that enables saving and loading up to 9 settings/effects with keyboard shortcuts for quick switching.

---

### 🪧 DEMO
* [Latest Version](https://adelando.net/projects/visualizer.html) *Stable-Latest version on Github*

* [WIP Version](https://adelando.net/projects/beta_visualizer.html). *Potentially Buggy - Potentially Messy*

---
## 🚀 Quick Start
1. **Open** the HTML file in any modern browser.
2. On **Chromium Browsers**  
   Click <ins>**[System Audio Capture]**</ins> *(for internal sound or applications or tabs)* or  
   On **Mobile or non-chromium browsers**  
   Click <ins>**[Microphone Input]**</ins> *(For enviromental sounds)*.
3. If using <ins>**System Audio**</ins>, ensure the <ins>**"Share Audio"**</ins> toggle is enabled in the Chromium browser popup.
4. Adjust your settings, colours and effects from the dropdown and sliders to customise to how you want.
5. Press **F11** for the full-screen experience.

---

## 🎛️ Control Manual

### **Core Rendering**
* **Gain / Sensitivity:** Multiplier for the audio input. Turn up for quiet tracks *(Default: 1)*.
* **Base Spacing:** Sets the initial gap between shapes/bars. *(Default: 10)*
* **Line Thickness:** Controls the width of the lines. *(Default: 2.0)*
    * *Note: Includes a dynamic buffer ($Spacing + (Thickness \times 1.5)$) to prevent overlapping.*
* **Complexity:** Determines how many rings or kaleidoscope slices are rendered. *(Default: 24)*
* **Rotation:** The speed at which the entire canvas spins. *(Default: 0.004)*
    * *Note: Positive value will rotate clockwise, Negitive value will rotate anti-clockwise.*
* **Master Zoom:** Overall scale of the visual. *(Default: 1.5)*
* **Decay (Trails):** Controls how long previous frames linger. *(Default: 0.50)*
    * *Note: Low = High Blur; High = Sharp Lines.*


## 🎨 Effect Breakdown & Logic
Not every setting affects every shape. Use the table below to understand the unique behavior of each mode.

| Effect Name | Logic Description | Ignores These Settings |
| :--- | :--- | :--- |
| **🛰️ Orbiting Moons** | Stars orbiting a central point. Reacts by jumping outward from orbit. | **Invert Toggle**, *(Invert only reverses rotation)* |
| **🍭 Kaleidoscope** | Mirrored bar patterns rotated around a central axis. | *Responds to all settings* |
| **🔺 Triangles** | Concentric geometric triangles pulsing to the bass. | *Responds to all settings* |
| **🔹 Hexagons** | Symmetrical 6-sided polygons with adaptive spacing. | *Responds to all settings* |
| **🔘 Circles** | Classic concentric rings. Best for "tunnel" effects. | **Rotation Speed** |
| **▪️ Squares** | Nested boxes. Great for architectural visuals. | *Responds to all settings* |
| **📊 Mirror Bar** | Traditional frequency bars mirrored on the X-axis. | **Rotation Speed, Invert Toggle** |
| **🔉 Waveform** | Direct time-domain representation of the audio signal. | **Invert Toggle, Complexity, Base Spacing** |

---

### **Color & Style**
* **Color Mode:** Choose between Rainbow or 5 specialized palettes (Cyberpunk, Lava, etc.).
* **Custom Palette:** Allows you to pick two specific colors to blend between.
* **Color Speed:** How fast the hues cycle through the spectrum.

---

## 💾 Preset Manager
* **Preset Bank:** 9 slots of local storage that persist even if you refresh the page.
    * *Keys **[1] through [9]:** Instantly load the corresponding Preset Slot.*
* **Export:** Converts your current masterpiece into a Base64 string. Share this code with others!
* **Import:** Paste a code into the box to instantly replicate someone else's settings.

Exporting your settings will provide a Base64 string like the below example.
```yaml
eyJzZW5zaXRpdml0eSI6IjEuMyIsImJhclNwYWNpbmciOjEsInRoaWNrbmVzcyI6IjQiLCJzbGljZXMiOiIzIiwicm90YXRpb24iOiIwIiwiem9vbSI6IjEuMyIsImRlY2F5IjoiMSIsIm1pcnJvckZsaXAiOnRydWUsInJhaW5ib3dTcGVlZCI6MSwiYmdDb2xvciI6IiMzODAwZDEiLCJyZWFjdGl2ZUJHIjp0cnVlLCJiYXNlU2hhcGUiOiJ0ZXh0IiwiY29sb3JNb2RlIjoiY3VzdG9tIiwiY29sb3IxIjoiIzAwZmJmZiIsImNvbG9yMiI6IiNmZjAwZmYiLCJjdXN0b21UZXh0IjoiQURFTEFORE8ifQ==
```
Which when [decoded](https://www.base64decode.org/) will result in a string.
```yaml
{"sensitivity":"1.3","barSpacing":1,"thickness":"4","slices":"3","rotation":"0","zoom":"1.3","decay":"1","mirrorFlip":true,"rainbowSpeed":1,"bgColor":"#3800d1","reactiveBG":true,"baseShape":"text","colorMode":"custom","color1":"#00fbff","color2":"#ff00ff","customText":"ADELANDO"}
```
Allowing you to edit or save in a text document outside the visualiser for later.

---

## 🛠️ Project Goals
Created by **Adelando**, this project aims to provide a zero-latency visual solution that requires no software installation. 

**Future Roadmap:**
* [ ] ?
* [ ] ?

**Found a bug?** Open an issue on the [GitHub Repository](https://github.com/adelando/webpage-audio-visualizer).
