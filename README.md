# 🎨 Gesture-Controlled 3D Particle Playground

A fun yet technically rich interactive web project built using **AI hand tracking, creative coding, and real-time 3D graphics**.  
This playground allows users to control thousands of particles using **natural hand gestures** captured through a webcam.

The project explores how **human motion** can directly influence **digital systems**, blending AI with visual art and physics-inspired behavior.

---

## ✨ Demo Highlights

- 20,000+ real-time animated particles  
- Gesture-based interaction using hand tracking  
- Smooth shape morphing and transitions  
- GPU-accelerated rendering with custom shaders  
- Works directly in the browser (no installation)

---

## 🧠 Core Idea

Instead of traditional mouse or keyboard input, this project uses **hand gestures** as the primary control mechanism.  
The goal is to experiment with **intuitive human-computer interaction** and show how AI can power creative, expressive interfaces.

---

## 🖐️ Gesture Controls

| Gesture | Action |
|------|------|
| Open hand vs fist | Controls particle spread and expansion |
| Hands closer / farther | Controls global scale (zoom) |
| Move hands left / right | Rotates the particle system |
| Quick snap motion | Triggers a fireworks burst |
| No camera available | Falls back to GUI + mouse controls |

---

## 🎛️ User Controls (Fallback)

If camera access is unavailable:
- `dat.GUI` sliders allow manual control of:
  - Particle count
  - Particle size
  - Color themes
  - Spread and scale
  - Rotation speed
- Mouse or touch drag rotates the scene

---

## 🌌 Particle Templates

The system supports multiple dynamic templates:

- ❤️ **Heart** – cardioid-based particle distribution  
- 🌸 **Flower / Sphere** – Fibonacci sphere for even spacing  
- 🪐 **Saturn** – ring system with central sphere  
- 💥 **Fireworks** – physics-inspired explosion with gravity and damping  

Particles smoothly morph between templates using interpolation and shader-based transitions.

---

## ⚙️ Technical Architecture

### 🔹 AI & Hand Tracking
- Uses **MediaPipe Hands** via TensorFlow.js  
- Extracts 3D hand landmarks in real time  
- Gesture logic derived from:
  - Finger tension
  - Wrist distance
  - Hand center position

### 🔹 Graphics & Rendering
- **Three.js** for scene management and rendering  
- **WebGL ShaderMaterial** for high-performance particles  
- Custom **GLSL vertex and fragment shaders** for:
  - Organic motion
  - Glow effects
  - Smooth transparency blending

### 🔹 Performance
- GPU-accelerated rendering  
- Efficient BufferGeometry usage  
- Adjustable particle count (up to 50,000)

---

## 🧩 Tech Stack

- **JavaScript (ES6)**
- **Three.js**
- **WebGL**
- **GLSL Shaders**
- **MediaPipe Hands**
- **TensorFlow.js**
- **dat.GUI**

---

## 🚀 How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/your-username/gesture-particle-playground.git
