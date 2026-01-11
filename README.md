# PSA Source Engine - Perfect Sensitivity Finder

**PSA Source Engine** is a high-performance, web-based aim sensitivity calculator and trainer built specifically for **Counter-Strike 2 (CS2)** and other **Source Engine** titles. It leverages a 7-iteration Perfect Sensitivity Approximation (PSA) algorithm within a custom 3D WebGL environment to help players discover their mathematically ideal in-game sensitivity.

## 🚀 Key Features

* **3D PSA Testing Environment:** Developed with `Three.js` to simulate actual in-game mouse movement, target tracking, and flicking.
* **Iterative PSA Algorithm:** A 7-step process that compares "High" vs "Low" sensitivity iterations to narrow down your optimal settings based on real-time performance.
* **Method B (360° Physical Calibration):** A unique tool that calculates base sensitivity by measuring the physical width of your mousepad.
* **CS2 Accurate Math:** Uses the industry-standard Source Engine yaw constant of $0.022$ to ensure 1:1 parity with in-game settings.
* **Physical Metrics:** Provides real-time calculation of your $cm/360$ (centimeters required for a full 360-degree turn).
* **Multi-Language Support:** Fully localized in English, Russian, Turkish, and Ukrainian.

## 🛠️ How It Works

1. **Initial Setup:** Enter your Mouse DPI and desired FOV (Default CS2 is 90).
2. **Calibration:**
    * **Method A:** Enter your current Source/CS2 sensitivity directly.
    * **Method B:** Select "Method B," place your mouse at the edge of your mat, drag it to the opposite edge, and press `ESC` to calculate your base sensitivity.
3. **The PSA Test:**
    * The engine runs 7 rounds.
    * In each round, you test two sensitivities (LOW and HIGH) for 15 seconds each.
    * Track and flick to the moving targets to earn points.
4. **Final Results:** The system provides your "Perfect Sensitivity" and the corresponding physical $cm/360$.

## 🎯 Post-Test Fine-Tuning

If the result feels slightly off in a live match, follow these guidelines provided by the tool:
* **Overshooting:** If your crosshair consistently passes the target during flicking, lower your result by $0.05 - 0.1$.
* **Undershooting:** If your movement feels sluggish or you fail to reach the target, raise your result by $0.05 - 0.1$.

## 💻 Technical Stack

* **Logic:** JavaScript (ES6+).
* **3D Rendering:** Three.js (WebGL).
* **Input:** Pointer Lock API for raw mouse data simulation.
* **UI:** Modern CSS3 with Glassmorphism effects.

---
**Developed by [Adiru3](https://github.com/Adiru3)**
