# 🌈 CHROMIUM WEB AUDIO VISUALIZER

![Visualizer Header](https://img.shields.io/badge/Status-Stable-brightgreen)
![VJ Ready](https://img.shields.io/badge/VJ-Ready-ff00ff)  

*Wish Spotify, Apple Music, or Youtube Music had a fullscreen visualizer for your party or event?*

A high-fidelity, browser-based, audio reactive tool designed to produce amazing visuals that are extremely customizable.  
Features a <ins>**Preset Manager**</ins> and a dynamic **Shortcut System** for live performance and quick switching.

---

### 🪧 DEMO
* [Latest Version](https://adelando.net/projects/visualizer.html) *Stable-Latest version on Github*

* [WIP Version](https://adelando.net/projects/beta_visualizer.html). *Potentially Buggy - Potentially Messy*

---
## 🚀 Quick Start
1. **Open** the HTML file in any modern browser.
2. **Audio Setup Guide:** Expand this section in the menu to find capture buttons.
   * On **Chromium Browsers**: Click <ins>**[System Audio Capture]**</ins> and ensure **"Also share tab audio"** is toggled **ON**.
   * On **Mobile/Others**: Click <ins>**[Microphone Input]**</ins> for environmental response.
3. **Customize:** Use the sliders or the new **Key+Arrow** shortcuts to tweak the effect.
4. **Reset:** If things get too wild, a **[Reset Sliders]** button appears at the bottom to return to defaults.
5. Press **F11** for the full-screen experience.

---

## 🎛️ Control Manual

### **Core Rendering**
* **Gain / Sensitivity (G):** Multiplier for audio input. *(Default: 1.0)*
* **Base Spacing (S):** Sets the gap between shapes or text iterations. *(Default: 10)*
* **Line Thickness (T):** Width of lines or size of text. *(Default: 2.0)*
* **Complexity (C):** Number of rings, slices, or vertical text clones. *(Default: 25)*
* **Rotation (R):** Canvas spin speed. Negative = Anti-clockwise. *(Default: 0.004)*
* **Master Zoom (Z):** Overall scale of the visual. *(Default: 1.5)*
* **Decay (D):** Trail length. Low = High blur; High = Sharp motion. *(Default: 0.50)*

### **⌨️ Keyboard Shortcuts**
Hold the letter key and press **Arrow Up/Down** or **Left/Right** to adjust:
* **G**: Gain | **S**: Spacing | **T**: Thickness | **C**: Complexity | **R**: Rotation | **Z**: Zoom | **D**: Decay
* **F**: Toggle Invert/Flip (Instant)
* **Q**: Toggle Reset to Defaults (Instant)
* **[1-9]**: Load Preset Slots

---

## 🎨 Effect Breakdown & Logic
| Effect Name | Logic Description | Unique Behavior |
| :--- | :--- | :--- |
| **🛰️ Orbiting Moons** | Stars orbiting a central point. | Reacts by jumping outward from orbit. |
| **🧠 Neural Web** | Physics-based nodes connected by reactive lines. | Lines thicken and nodes speed up on beats. |
| **🔠 Custom Text** | Displays a custom string with a see-saw wobble. | **Rotation Speed** is ignored. Scales up to 150%. |
| **🍭 Kaleidoscope** | Mirrored bar patterns rotated around an axis. | Complexity controls the number of "slices." |
| **🔺 Triangles** | Concentric geometric triangles. | Pulses to low-end frequencies. |
| **🔹 Hexagons** | Symmetrical 6-sided polygons. | Clean geometric tunnel effect. |
| **🔘 Circles** | Classic concentric rings. | Best for minimalist tunnel visuals. |
| **▪️ Squares** | Nested boxes. | Great for architectural/grid visuals. |
| **📊 Mirror Bar** | Traditional frequency bars mirrored on the X-axis. | Rotation and Invert are generally ignored. |
| **🔉 Waveform** | Direct time-domain signal representation. | Ignores Complexity and Spacing. |

---

## 💾 Preset Manager
* **Preset Bank:** 9 slots of local storage that persist even if you refresh the page.
* **Export:** Converts your current masterpiece into a Base64 string.
* **Import:** Paste a code into the box to instantly replicate a preset.

---

## 🛠️ Project Goals
Created by **Adelando**, this project aims to provide a zero-latency visual solution that requires no software installation. 

**Future Roadmap:**
* [ ] ??
* [ ] ??

---

<details>
<summary>📂 <b>MY FAVOURITE COMBINATIONS SO FAR</b></summary>


### 🔠 Name Shadow Drop
![Example](https://i.imgur.com/QFekUht.png) 
<details>  
<summary>View example code: </summary>
  
`eyJzZW5zaXRpdml0eSI6IjEuNiIsImJhclNwYWNpbmciOiIxIiwidGhpY2tuZXNzIjoiMi41Iiwic2xpY2VzIjoiNCIsInJvdGF0aW9uIjowLjAwNCwiem9vbSI6IjEuOCIsImRlY2F5IjoiMSIsIm1pcnJvckZsaXAiOnRydWUsInJhaW5ib3dTcGVlZCI6IjAiLCJiZ0NvbG9yIjoiIzAwODFmYSIsInJlYWN0aXZlQkciOnRydWUsImJhc2VTaGFwZSI6InRleHQiLCJjb2xvck1vZGUiOiJjdXN0b20iLCJjb2xvcjEiOiIjMDZmYWZlIiwiY29sb3IyIjoiIzAwMDAwMCIsImN1c3RvbVRleHQiOiJBREVMQU5ETyJ9`

</details>

*Description: Colour Speed=0, Custom colour (1st=Cyan #06fafe / 2nd=Black #000000), Spacing=1, Complexity=4*

### 🌌 Neon Neural Web
![Example](https://i.imgur.com/Z13zl8i.png)  

<details>  
<summary>View example code: </summary>
  
`eyJzZW5zaXRpdml0eSI6IjIuMSIsImJhclNwYWNpbmciOiIxNSIsInRoaWNrbmVzcyI6IjEiLCJzbGljZXMiOiI2OSIsInJvdGF0aW9uIjoiLTAuMDA2Iiwiem9vbSI6IjEuNyIsImRlY2F5IjoiMC4wOSIsIm1pcnJvckZsaXAiOmZhbHNlLCJyYWluYm93U3BlZWQiOiIwLjIiLCJiZ0NvbG9yIjoiIzAwMDAwMCIsInJlYWN0aXZlQkciOmZhbHNlLCJiYXNlU2hhcGUiOiJuZXVyYWwiLCJjb2xvck1vZGUiOiJjeWJlciIsImNvbG9yMSI6IiMwNmZhZmUiLCJjb2xvcjIiOiIjZjQwMWViIiwiY3VzdG9tVGV4dCI6IuKKgijil4nigL/il4kp44GkIn0=`  

</details>

*Description: High decay 0.09, Cyberpunk Colour palette.*

### 🚀 Firey Orbit

![Example]([https://i.imgur.com/Z13zl8i.png](https://i.imgur.com/3MrLxUN.png))  
<details>  
<summary>View example code: </summary>
  
`eyJzZW5zaXRpdml0eSI6IjAuNCIsImJhclNwYWNpbmciOiIzIiwidGhpY2tuZXNzIjoiMC41Iiwic2xpY2VzIjoiMiIsInJvdGF0aW9uIjoiMC4wMTEiLCJ6b29tIjoiMS41IiwiZGVjYXkiOiIwLjI0IiwibWlycm9yRmxpcCI6ZmFsc2UsInJhaW5ib3dTcGVlZCI6MSwiYmdDb2xvciI6IiMwMDAwMDAiLCJyZWFjdGl2ZUJHIjpmYWxzZSwiYmFzZVNoYXBlIjoibW9vbnMiLCJjb2xvck1vZGUiOiJsYXZhIiwiY29sb3IxIjoiI2ZmZmZmZiIsImNvbG9yMiI6IiNmZmZmZmYiLCJjdXN0b21UZXh0Ijoi4oqCKOKXieKAv+KXiSnjgaQifQ==`  

</details>

*Description: Zoomed out, dense spacing, Lava Flow Colour palette*

</details>

---

**Found a bug?** [Open an issue here](https://github.com/adelando/webpage-audio-visualizer/issues).
