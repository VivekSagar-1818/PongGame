# Pong Game (Raylib C++)


A classic 2-player arcade **Pong Game** built in C++ using the [Raylib](https://www.raylib.com/) library. It features smooth 60 FPS gameplay, circle-to-rectangle paddle collisions, a custom fading intro sequence, real-time score tracking, and local two-player keyboard controls.

---

## Features

- **Animated Intro Screen:** Displays a fading `"PONG GAME!"` title card on launch that transitions smoothly using alpha blending (`Fade`) before the match begins.
- **Dynamic Ball Physics & Collisions:**
  - Accurate circle-to-box collision detection (`CheckCollisionCircleRec`) against both paddles.
  - Boundary bouncing on top and bottom window edges.
- **Live Scoreboard:** Tracks and displays individual scores for Player 1 and Player 2 in real time with high-visibility yellow counters.
- **Two-Player Local Controls:** Independent, responsive paddle movement bounded strictly within the screen height.

---

## Technical Specifications

| Parameter | Value |
| :--- | :--- |
| **Window Dimensions** | 1200 × 800 pixels |
| **Target Frame Rate** | 60 FPS |
| **Ball Radius** | 10 pixels |
| **Ball Speed** | $v_x = 5$, $v_y = -5$ |
| **Paddle Size** | 20 × 225 pixels |
| **Paddle Move Speed** | 10 px/frame |
| **Language** | C++ |
| **Graphics Framework** | Raylib |

---

## Game Controls

| Player | Up Key | Down Key |
| :--- | :--- | :--- |
| **Player 1 (Left Paddle)** | `W` | `S` |
| **Player 2 (Right Paddle)** | `Up Arrow` | `Down Arrow` |

- **Exit:** `Escape` or click the window close button.

---

## Project Structure

```text
PongGame/
├── demo.gif         # Gameplay preview animation
├── PongGame.cpp     # Complete game loop, physics, input, and render logic
└── README.md        # Project documentation
