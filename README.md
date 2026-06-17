# FortniteAssistantAI
<p align="center">
  <a href="https://github.com/aipsofters/FortniteAssistantAI/releases/latest">
    <img src="https://img.shields.io/badge/DOWNLOAD-LAUNCHER_v1.0.0-00ff66?style=for-the-badge&logo=windows&logoColor=1a1a2e&labelColor=1a1a2e" alt="Download FortniteAssistantAI" height="45">
  </a>
</p>
---
##  Technical Stack & Pipeline
# FortniteAssistantAI: Advanced Computer Vision & Input Optimization Framework for Fortnite Environments

FortniteAssistantAI is a high-performance, non-intrusive accessibility and analytics suite built using custom-trained neural networks. It is specifically optimized to analyze the fast-paced, high-verticality environment of *Fortnite* (including Battle Royale and Creative modes), providing real-time spatial awareness and input alignment.

> **Legal & Educational Disclaimer:** This repository is maintained strictly for academic research, human-computer interaction analysis, and accessibility purposes. It does not manipulate game memory, modify game files, or inject code into the game client. Users are responsible for complying with the game's End User License Agreement (EULA).
<p align="center">
  <img src="https://github.com/user-attachments/assets/5e958565-0857-44f9-9966-1a7294e470f1" width="600" alt="Spatial Telemetry Overlay">
</p>
---

##  Core Features & Technical Capabilities

### 1. Dynamic Model Recognition (Visual Assistance)
Instead of interacting with game memory (Internal), the engine uses an **External Pixel-Analysis Pipeline** to identify distinct geometric shapes, character player models (Skins), and build structures unique to *Fortnite*'s art style.
* **Building & Edit Visual Aid:** Isolates player silhouettes amidst dense building structures or custom edits.
* **Distance Approximation:** Leverages bounding-box scaling to calculate real-time distance metrics of moving entities.
<p align="center">
  <img src="https://github.com/user-attachments/assets/aa67c5eb-84a5-4e7b-8b0f-166277e2fe33" width="600" alt="Spatial Telemetry Overlay">
</p>
### 2. Low-Latency Input Alignment Vector (Dynamic Tracking)
Calculates the spatial discrepancy between the user's current camera vector and the detected target matrix. 
* **Humanized Smoothing:** Uses advanced Bezier curve interpolation to prevent robotic movements, emulating organic human input.
* **FOV (Field of View) Zoning:** Allows users to define a strict pixel radius ($R_{fov}$) for tracking activation to prevent erratic shifts during rapid build-fights.

### 3. Tactical Spatial Overlay (Augmented Reality HUD)
Renders a lightweight, transparent vector overlay directly onto the Windows Desktop Window Manager (DWM).
* **Entity Telemetry:** Displays bounding frames around detected player models.
* **Weapon Bloom & Recoil Compensation Assistance:** Provides static visual reference points to assist players in managing weapon spread patterns during bloom-heavy Fortnite gunplay.
<p align="center">
  <img src="https://github.com/user-attachments/assets/0ee09844-c63b-4222-a6aa-d43b9d157788" width="600" alt="Spatial Telemetry Overlay">
</p>
---

##  Architectural Blueprint & Math

The framework captures the screen at high refresh rates (144Hz+) and processes frames through a lightweight, custom-weighted inference engine.

The core alignment delta vector $\vec{A}$ is determined by calculating the distance between the camera center $(X_{c}, Y_{c})$ and the optimized target coordinate $(X_{t}, Y_{t})$ adjusted by a dynamic damping coefficient $k$:

$$\vec{A} = k \cdot \left( \begin{matrix} X_{t} - X_{c} \\ Y_{t} - Y_{c} \end{matrix} \right)$$

Where $k$ acts as the **Smoothing/Humanization Factor** to guarantee fluid, natural behavioral emulation.
<p align="center">
  <img src="https://github.com/user-attachments/assets/f9d4b9ac-9b9c-452d-ad87-8789f0feaf64" width="600" alt="Spatial Telemetry Overlay">
</p>
---

##  Deployment & Configuration

### Prerequisites
* NVIDIA GPU with CUDA Core support (highly recommended for sub-5ms inference times).
* Python 3.10+ environment.
<p align="center">
  <img src="https://img.shields.io/github/stars/aipsofters/FortniteAssistantAI?style=for-the-badge&color=00ff66&labelColor=1a1a2e" alt="Stars">
  <img src="https://img.shields.io/github/forks/aipsofters/FortniteAssistantAI?style=for-the-badge&color=7b2cbf&labelColor=1a1a2e" alt="Forks">
  <img src="https://img.shields.io/github/license/aipsofters/FortniteAssistantAI?style=for-the-badge&color=ff007f&labelColor=1a1a2e" alt="License">
</p>

---

##  System Interface Preview
> **Bento Grid Design** featuring high-contrast static analytical overlays, neon aesthetics, and a custom hardware-accelerated initialization sequence.
---

##  Key Architectural Modules

* **Dynamic Object Tracking:** Real-time multi-class asset detection utilizing localized bounding box generation optimized for rapid-motion environments.
* **Spatial Trajectory Modeling:** Advanced mathematical processing of screen-space vectors to analyze structural environments and entity positioning.
* **Glassmorphic Matrix UI:** A streamlined, static-background cyberpunk interface built on **PySide6** with enhanced readability for high-intensity sessions.
* **Fault-Tolerant Diagnostics:** Real-time execution logging backed by a dedicated telemetry verification routine.
​
​
