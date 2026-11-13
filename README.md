# AI-Rock-Paper-Scissiors
A web Rock Paper Scissors game where you have to play against an AI. Instead of choosing the move you have to show the gesture to the camera. A game where you dont have to even touch ypur keyboard to win.


# HumaityVersusAIBattleOfTheCentury – Documentation

## 1. Overview
Gesture Game is a browser-based Rock, Paper, Scissors game where the player competes against an AI opponent using hand gestures detected through their webcam. The objective is to defeat the AI by reducing its health to zero before the player's health reaches zero.

## 2. Technologies Used
- **JavaScript** – Implements the game logic and functionality.
- **p5.js** – Handles the webcam feed, canvas and visual elements.
- **MediaPipe Gesture Recognizer** – Detects and recognises the player's hand gestures.
- **HTML/CSS** – Provides the game structure and interface.

## 3. How to Play
1. Allow the game to access your webcam.
2. Read the instructions displayed when the game starts.
3. Show a thumbs-up to begin.
4. Show another thumbs-up to start the countdown.
5. Once the countdown finishes, make one of the three recognised gestures.
6. The AI randomly selects its own gesture, and the winner deals damage.
7. Continue playing until either the player or the AI runs out of health.

## 4. Recognised Gestures

| Hand Gesture | Action |
|---|---|
| ✌️ Victory | Scissors |
| ✋ Open Palm | Paper |
| ✊ Closed Fist | Rock |
| 👍 Thumbs Up | Start / Continue |
| 👎 Thumbs Down | Restart |

## 5. Game Rules
The game follows the traditional Rock, Paper, Scissors rules:

- Rock beats Scissors.
- Scissors beats Paper.
- Paper beats Rock.

Both the player and AI start with **1,000 health points**.

Each successful attack deals 100 damage multiplied by the current damage multiplier.

- **Winning:** Increases the winner's damage multiplier for the next round.
- **Losing:** Resets the player's multiplier and increases the AI's multiplier.
- **Drawing:** Doubles the damage multiplier for the next round.

## 6. Main Features
- Real-time hand gesture recognition using a webcam.
- AI opponent with randomly generated moves.
- Health bars and damage multiplier system.
- Countdown before each round.
- Visual animations and dynamic AI portraits.
- Restart functionality using hand gestures.
- On-screen instructions and game announcements.

## 7. Technical Implementation
The game is organised into five main sections:

1. **Variables:** Stores game state, health, multipliers and gesture recognition variables.
2. **Setup:** Initialises the webcam, loads the MediaPipe model and creates the interface.
3. **Game System:** Controls the game loop, rounds, countdown, gesture recognition and damage calculation.
4. **Helpers:** Contains reusable functions for gesture detection, game evaluation and background changes.
5. **Interface:** Manages health bars, multipliers, announcements and other visual elements.

## 8. Requirements
- A modern web browser.
- A working webcam.
- Internet connection to load p5.js, MediaPipe and the gesture recognition model.
- Webcam permissions enabled.


