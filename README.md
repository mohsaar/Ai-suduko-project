# 🎮 Sudoku Game with Flask and AI (DFS + Backtracking)

## 🧠 Overview

This is a fully functional and interactive **Sudoku game** built with:
- 🐍 **Python + Flask** (Backend)
- 🎨 **HTML, CSS, JavaScript** (Frontend)
- 🤖 **AI algorithms** (Depth-First Search + Backtracking) to solve puzzles

---

## 💡 Features

✅ 5 Difficulty Levels: Beginner, Easy, Medium, Hard, Expert  
✅ Clean and responsive UI  
✅ Auto-solver with step-by-step visual explanation  
✅ Hint system and timer  
✅ Input validation (accepts only numbers 1–9)

---

## 🧩 How It Works

### 🔢 1. Sudoku Board Generation
- A complete board is generated, then numbers are removed based on difficulty:

| Difficulty | Empty Cells |
|------------|-------------|
| Beginner   | 30 - 35     |
| Expert     | 54 - 60     |

### 🕹️ 2. Game Interface
- Interactive 9×9 grid
- Control buttons: Hint – Check – Show Solution – Visualize Solving
- Real-time timer and stats display

### 🤖 3. Solving Algorithm (DFS + Backtracking)
1. Find the next empty cell
2. Try numbers from 1 to 9
3. Check validity (row, column, 3x3 box)
4. Backtrack if needed when no valid options remain

---

## 🛠️ Project Structure

Sudoku/
├── Sodo.py # Flask server
├── requirements.txt # Python dependencies
├── templates/
│ ├── game.html # Game interface
│ ├── levels.html # Difficulty selection page
│ ├── solution.html # Final solution view
│ └── congrats.html # Victory screen
├── static/
│ ├── css/styles.css # Styling
│ └── js/game.js # Game logic (timer, validation, interactivity)

## ▶️ How to Run Locally

1. Install Flask:
```bash
pip install Flask

## Run the server:
python Sodo.py
