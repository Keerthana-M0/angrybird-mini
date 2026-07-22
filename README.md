# 🐦 AngryBird Mini

> A miniature Angry Birds-inspired game built with **C++** and **SFML** featuring projectile physics, gravity, destructible blocks, and collision detection.

![C++](https://img.shields.io/badge/C%2B%2B-17-blue.svg)
![SFML](https://img.shields.io/badge/SFML-2.5+-green.svg)


---

## 📸 Preview

<p align="center">
  <img src="images/gameplay.png" width="700">
</p>

*(Replace with a screenshot or GIF.)*

---

## ✨ Features

- 🎯 Slingshot aiming
- 🐦 Projectile motion
- 🌍 Gravity simulation
- 🧱 Destructible blocks
- 💥 Collision detection
- 👾 Enemy target
- 🏆 Win condition
- 🔁 Restart support
- 📈 Score tracking
- 📍 Trajectory prediction

---

## 🎮 Controls

| Action | Key |
|---------|-----|
| Aim | Click & Drag |
| Shoot | Release Mouse |
| Restart | R |
| Quit | Close Window |

---

## 🛠 Tech Stack

- C++17
- SFML 2.5+
- CMake

---

## 📂 Project Structure

```text
AngryBirdMini/
│
├── src/
│   └── main.cpp
│
├── CMakeLists.txt
├── README.md
└── .gitignore
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/<username>/AngryBirdMini.git
cd AngryBirdMini
```

### Build

```bash
cmake -S . -B build
cmake --build build
```

### Run

Linux

```bash
./build/AngryBirdMini
```

Windows

```text
build\Debug\AngryBirdMini.exe
```

---

## 🎯 Gameplay

### Slingshot

```cpp
sf::Vector2f drag = startPosition - bird.getPosition();
bird.velocity = drag * LAUNCH_POWER;
```

---

### Gravity

```cpp
velocity.y += GRAVITY * deltaTime;
position += velocity * deltaTime;
```

---

### Block Collision

```cpp
if (impactSpeed > 250.f)
    block.damage(1);
```

---

## 🧠 Concepts Used

- Object-Oriented Programming
- Game Loop
- Physics Simulation
- Projectile Motion
- Collision Detection
- Vector Mathematics
- Event Handling

---

## 🚀 Future Improvements

- Multiple birds
- Multiple levels
- Sound effects
- Animations
- Particle effects
- Box2D physics
- Level editor
- Save system

---

