# 🚀 Space Shooter Game (Java OOP)

A 2D Space Shooter game built in **Java** using **Swing/AWT**, developed as a semester project to demonstrate core **Object-Oriented Programming (OOP)** concepts.

---

## 🎮 Features

- Wave-based enemy spawning system (gets harder every wave)
- 3 enemy types: **Basic Enemy**, **Fast Enemy**, and **Boss Enemy**
- Boss fight every 3rd wave with a 3-bullet spread attack
- Player health, lives, and score system
- Animated main menu with custom Swing buttons
- Game Over screen with final score & player rating
- Smooth 60 FPS game loop using `Thread` + `Runnable`
- AABB collision detection
- Scrolling parallax star background

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Java SE (JDK 8+) | Core language |
| Java Swing / AWT | GUI, rendering, buttons |
| Eclipse IDE | Development environment |

---

## 🧩 OOP Concepts Demonstrated

| Concept | Where Used |
|---------|-----------|
| **Inheritance** | `Player`, `Bullet`, `Explosion` → `GameObject`; `BasicEnemy`, `FastEnemy`, `BossEnemy` → `Enemy` → `GameObject` |
| **Polymorphism** | `render()`, `update()`, `move()`, `shoot()` overridden differently in each class |
| **Encapsulation** | All fields `private`, accessed via getters/setters |
| **Abstraction** | `GameObject` and `Enemy` are abstract classes with abstract methods |
| **Interfaces** | `Shootable` and `Damageable` implemented by `Player` and `Enemy` subclasses |
| **Swing & Buttons** | `JFrame`, `JPanel`, custom-styled `JButton` in Menu & Game Over screens |

---

## 📁 Project Structure

```
SpaceShooter/
└── src/
    └── spaceshooter/
        ├── SpaceShooterGame.java   # Main entry point (JFrame)
        ├── GameObject.java         # Abstract base class
        ├── Shootable.java          # Interface
        ├── Damageable.java         # Interface
        ├── Player.java             # Player ship
        ├── Bullet.java             # Projectiles
        ├── Enemy.java              # Abstract enemy base
        ├── BasicEnemy.java         # Wavy purple enemy
        ├── FastEnemy.java          # Fast bouncing enemy
        ├── BossEnemy.java          # Boss with spread attack
        ├── Explosion.java          # Explosion VFX
        ├── StarBackground.java     # Scrolling stars
        ├── GamePanel.java          # Game loop & rendering
        ├── MenuPanel.java          # Main menu
        └── GameOverPanel.java      # Game over screen
```

---

## ▶️ How to Run

### Option 1: Eclipse IDE
1. Clone or download this repository
2. Open Eclipse → `File → Import → General → Existing Projects into Workspace`
3. Select the cloned folder
4. Right-click `SpaceShooterGame.java` → `Run As → Java Application`

### Option 2: Command Line
```bash
cd src
javac spaceshooter/*.java
java spaceshooter.SpaceShooterGame
```

---

## 🎹 Controls

| Key | Action |
|-----|--------|
| `Arrow Keys` / `W A S D` | Move ship |
| `SPACE` (hold) | Shoot (rapid fire) |
| `P` | Pause / Resume |
| `ESC` | Return to main menu |

---

## 🏆 Scoring & Ratings

| Enemy | Score |
|-------|-------|
| Basic Enemy | 100 pts |
| Fast Enemy | 150 pts |
| Boss Enemy | 1000 pts |

| Final Score | Rating |
|--------------|--------|
| 5000+ | ⭐⭐⭐ Ace Commander |
| 2000–4999 | ⭐⭐☆ Veteran Pilot |
| 800–1999 | ⭐☆☆ Rookie Pilot |
| 0–799 | ☆☆☆ Keep Training |

---

## 📸 Screenshots

| Main Menu     -----------------------------------   Gameplay        ----------------------------------         Game Over |

| <img width="250" height="200" alt="gameplay" src="https://github.com/user-attachments/assets/16eefab6-554d-40f1-ba29-cff229dd1866" /> | <img width="250" height="200" alt="gameplay" src="https://github.com/user-attachments/assets/7ea28f64-e8d6-45f8-b60a-a14b9e33d47b" />  <img width="250" height="200" alt="gameplay" src="https://github.com/user-attachments/assets/5fdeb1ad-7120-4624-8f69-61871e45f153" /> |

---

## 📄 License

This project is open-source and free to use for educational purposes.

---

## 👤 Author

**SAWAIRA QUDSIA**

Semester Project — Java OOP
