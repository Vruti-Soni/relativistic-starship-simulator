# relativistic-starship-simulator
# Relativistic Starship & Starfield Simulator
A high-performance, browser-based interactive 3D simulation exploring the visual and kinematic effects of **Special Relativity**. Built with **Three.js** and WebGL, this project models real-time **Relativistic Aberration** and **Spectral Doppler Shifting (Doppler Beaming)** across a 6,000-star field from the perspective of an accelerating starship.
---

## 🔬 Core Physics Implementations

Classical mechanics fail at relativistic velocities ($\beta = v/c \rightarrow 1$). This simulator solves relativistic kinematic transformations frame-by-frame for thousands of independent celestial light sources:

### 1. Relativistic Aberration (Angular Aberration of Light)
As the observer's velocity increases, incoming light rays bunch up toward the direction of motion (the "headlight effect"). The transformation of stellar direction vectors is computed using Lorentz velocity components:

$$x' = \frac{x}{\gamma (1 - \beta z)}, \quad y' = \frac{y}{\gamma (1 - \beta z)}, \quad z' = \frac{z - \beta}{1 - \beta z}$$

where $\gamma = \frac{1}{\sqrt{1 - \beta^2}}$ is the **Lorentz Factor**.

### 2. Relativistic Doppler Beaming & Spectral Shifting
Light frequency and intensity shift depending on the observer's relative motion and angle of approach. The Doppler factor $D$ dictates both frequency shifts and flux amplification:

$$D = \frac{1}{\gamma (1 - \beta \cos\theta)}$$

- **Blueshift ($D > 1$):** Stars appearing ahead of the vessel shift from white/yellow into brilliant cyan and ultraviolet spectra.
- **Redshift ($D < 1$):** Stars receding behind the vessel shift toward orange, red, and infrared wavelengths.

---

## 🎛️ Features & Controls

- **Interactive Velocity Slider:** Seamlessly accelerate your starship from rest up to $0.98c$ and observe real-time Lorentz contraction effects and time dilation ($\gamma t$).
- **Cinematic Camera Modes:** Toggle between **IMAX Track**, **Cockpit First-Person View**, and **Side Orbit** perspectives.
- **Telemetry HUD:** Live readout monitoring velocity ($\beta$), Lorentz factor ($\gamma$), and time dilation.

---
Result( https://vruti-soni.github.io/relativistic-starship-simulator/)
